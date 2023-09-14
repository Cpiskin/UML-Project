public class Dog {
    // Fields
    private String name;
    private String breed;
    private int age;

    // Constructors
    public Dog() {
        // Default constructor
    }

    public Dog(String name, String breed, int age) {
        this.name = name;
        this.breed = breed;
        this.age = age;
    }

    // Getter methods
    public String getName() {
        return name;
    }

    public String getBreed() {
        return breed;
    }

    public int getAge() {
        return age;
    }

    // Setter methods
    public void setName(String name) {
        this.name = name;
    }

    public void setBreed(String breed) {
        this.breed = breed;
    }

    public void setAge(int age) {
        this.age = age;
    }

    // toString method
    @Override
    public String toString() {
        return "Dog [name=" + name + ", breed=" + breed + ", age=" + age + "]";
    }

    // equals method
    public boolean equals(Dog otherDog) {
        return this.name.equals(otherDog.getName()) &&
               this.breed.equals(otherDog.getBreed()) &&
               this.age == otherDog.getAge();
    }
}
