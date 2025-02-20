# lab-5
//t2
class employee{

	String name;
	int id;
	double salary;

	employee (String name , int id, double salary){
		this.name=name;
		this.id=id;
		this.salary=salary;
	}

	public void incsal(float sal){
		salary+=sal;
		System.out.println("Increas Salary"+salary);
	}

	public void anualsal(){
		System.out.println("Annual Salary"+salary*12);
	}

	public void display(){
		System.out.println("Name : "+name);
		System.out.println("ID : "+id);
		System.out.println("Salary : "+salary);

	}

public static void main(String[]args){

	employee e1=new employee("Hanan ",146, 14000.0);
	
	e1.incsal(1000);
	e1.display();
	e1.anualsal();
}
}

//t1

class book{
 	
    String title ="Oliver twist";
    String author = "charles dawkins";
    boolean isavail=true;
    
    public void borrowbook(){
      isavail=false;
      if(isavail){
        isavail=true;
      	System.out.println("Book is available ");
      }else{
        System.out.println("Book is borrwed");
      }

    }
    public void returnbook(){
    if(isavail){
     }else{
        isavail=true;
     }
 
    }
    public void displaybook(){
    
    System.out.println("Title : "+title);
    System.out.println("Author : "+author);
    System.out.println("Available : "+isavail);

    }

    public static void main(String[] args){
    	book b1=new book();
        b1.displaybook();
        b1.borrowbook();
        b1.displaybook();

        b1.borrowbook();
        b1.returnbook();
        b1.displaybook();

    }
}
