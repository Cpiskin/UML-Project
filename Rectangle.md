public class Rectangle {
    // Fields
    private double length;
    private double width;
    private double angle;
    private int sides;
    private String name;

    // Constructors
    public Rectangle() {
        // Default constructor
    }

    public Rectangle(double length, double width) {
        this.length = length;
        this.width = width;
        this.angle = 90.0; // Assuming a right angle for simplicity
        this.sides = 4; // A rectangle has four sides
        this.name = "Rectangle";
    }

    // Getter methods
    public double getLength() {
        return length;
    }

    public double getWidth() {
        return width;
    }

    // Setter methods
    public void setLength(double length) {
        this.length = length;
    }

    public void setWidth(double width) {
        this.width = width;
    }

    // toString method
    @Override
    public String toString() {
        return "Rectangle [length=" + length + ", width=" + width + ", angle=" + angle +
                ", sides=" + sides + ", name=" + name + "]";
    }

    // equals method
    public boolean equals(Rectangle otherRectangle) {
        return this.length == otherRectangle.getLength() &&
               this.width == otherRectangle.getWidth();
    }

    // Additional methods
    public double getArea() {
        return length * width;
    }

    public double getPerimeter() {
        return 2 * (length + width);
    }
    }
    
