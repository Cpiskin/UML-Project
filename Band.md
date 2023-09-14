public class Band {
    // Fields
    private String artist;
    private int year;

    // Constructor
    public Band(String artist, int year) {
        this.artist = artist;
        this.year = year;
    }

    // Getter methods
    public String getArtist() {
        return artist;
    }

    public int getYear() {
        return year;
    }

    // Setter methods
    public void setArtist(String artist) {
        this.artist = artist;
    }

    public void setYear(int year) {
        this.year = year;
    }

    // toString method
    @Override
    public String toString() {
        return "Band [artist=" + artist + ", year=" + year + "]";
    }
}
