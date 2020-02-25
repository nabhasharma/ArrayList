# Checkng employee data
package Party;

import java.util.ArrayList;

public class Employee {
	String name;
	int age;
	
	public Employee(String name, int age) {
		
		this.name = name;
		this.age = age;
	}
	
	public String getName() {
		return name;
	}

	public void setName(String name) {
		this.name = name;
	}

	public int getAge() {
		return age;
	}

	public void setAge(int age) {
		this.age = age;
	}

	public boolean equals(Object obj) {
		Employee emp1=(Employee)obj;
		
		return this.name.equals(emp1.getName());
		
	}

	public static void main(String[] args) {
		ArrayList list=new ArrayList();
		Employee emp1=new Employee("mark",31);
		Employee emp2=new Employee("mark",32);
		Employee emp3=new Employee("carle",33);
		if(emp1.equals(emp2)) 
			System.out.println("Same");
			else
				System.out.println("not same");
		if(emp1.equals(emp3)) 
			System.out.println("Same");
			else
				System.out.println("not same");
	boolean found= list.contains(new Employee("mark",31));
	System.out.println(found);
	}
		
	}


