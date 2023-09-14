public class Square {
    // Fields
    private double side;

    // Constructor
    public Square(double side) {
        this.side = side;
    }

    // Getter methods
    public double getSide() {
        return side;
    }

    public double getLength() {
        return side;
    }

    public double getWidth() {
        return side;
    }

    // Setter methods
    public void setSide(double side) {
        this.side = side;
    }

    public void setLength(double side) {
        this.side = side;
    }

    public void setWidth(double side) {
        this.side = side;
    }

    // toString method
    @Override
    public String toString() {
        return "Square [side=" + side + "]";
    }

    // equals method (overriding equals from Rectangle)
    @Override
    public boolean equals(Object obj) {
        if (this == obj) return true;
        if (obj == null || getClass() != obj.getClass()) return false;

        Square square = (Square) obj;

        return Double.compare(square.side, side) == 0;
    }

    // Additional methods (overriding methods from Rectangle)
    public double getArea() {
        return side * side;
    }

    public double getPerimeter() {
        return 4 * side;
    }
}
