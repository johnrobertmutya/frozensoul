# frozensoul

public class Main {
    
    public static void main(String[] args) {
    		Person a = new Person(" Sung Jinwoo ");
    		Person b = new Person(" Coby Giant ");
    		//a.name = "xxxx";
    		//a.getage = 22;
    		//a.getAddress = "zzzz";
    		//b.name = "yyyy";
    		//b.getage = 25;
    		//b.getAddress = "rrr";
    		//a.greet = "Hi";
    		
    		System.out.println(a.getName());
    		System.out.println(b.getName());
    		a.setAge(22);
    		a.setAddress("25 diliman quezon city");
    		System.out.println(a.getAddress());
    		System.out.println(a.getAge());
    		b.setAge(26);
    		b.setAddress("30 diliman quezon city");
    		System.out.println(b.getAddress());
    		System.out.println(b.getAge());
    		a.greet(b);
    		a.greet(a);
    	   		
    }	
}
______________________________________________________
public class Person {
	private	String name = null;
	private	int age = 0;
	private String address = null;
	
	public String getName(){
		return this.name;
	}
	public int getAge(){
		return this.age;
	}
	public String getAddress(){
		return this.address;
	}
	public Person(String name){
	    this.name = name; 
	} 
	public void setName(String name){
		this.name = name;
	}
	public void setAge(int age){
		this.age = age;
	}
	public void setAddress(String address){
		this.address = address;
	}
	public void greet(Person P){
		System.out.println("Hi" + P.getName()+ "My name is " + this.name);
	}
    
}
