# Pen project
public class Pen
{
    //private instance variables - properties of the class
    private String color;
    private boolean erasable; 
    
    //full constructor - all parameters match instance varaibles
    public Pen(String c, boolean e)
    {
        //this on left matches the variables on top
        ///right variable matches the parenthesis
        this.color = c;
        this.erasable = e;
    }
    
    //accessor/getter - public, matching type from top
    public String getColor()
    {
        //just return instance variable
        return color;
    }
    
    //accessor/getter - public, matching type from top
    public boolean isErasable()
    {
        //just return instance variable
        return erasable;
    }
    
    //mutator/setter - public void, parameter in parenthesis matches variable from top
    public void setColor(String c)
    {
        this.color = c;
    }
    
    //mutator/setter - public void, parameter in parenthesis matches variable from top
    public void setErasable(boolean e)
    {
        this.erasable = e;
    }
 
    //return nicely formatted string(s) to display the instance variables from the top
    public String toString()
    {
        if(erasable)
        {
            return "Pen is " + color + " and can be erased.";
        }
        
        return "Pen is " + color + " and cannot be erased.";
    }
    
}
