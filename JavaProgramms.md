BigInteger program **********************

import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {

    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        BigInteger fno = new BigInteger(sc.next());
        BigInteger sno = new BigInteger(sc.next());
        System.out.println(fno.add(sno));
        System.out.println(fno.multiply(sno));
        
    }
}
******************************
number is prime or not 

import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {

   public static void main(String[] args) {
      Scanner in = new Scanner(System.in);
      BigInteger n = in.nextBigInteger();
      in.close();
      // Write your code here.
       if(n.isProbablePrime(1)){
           System.out.println("prime");
       }
       else{
           System.out.println("not prime");
       }
   }
} 

******************************
/* java programing notes on rivision time */
/*java tokenizer */
import java.util.*;
class stringTokenizer{
public static void main(String[] args){
String str=new String("bhagalpur college of engineering");
StringTokenizer st=new StringTokenizer(str);
int count=st.countTokens();
System.out.println("no of token is :"+count);
while(st.hasMoreTokens()){
	System.out.println(st.nextToken());
}
}
}

***************************

with multiple delimeter

import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String s = sc.nextLine();
        StringTokenizer st=new StringTokenizer(s," '.!,?_@");
        int counttoken=st.countTokens();
        System.out.println(counttoken);
        while(st.hasMoreTokens()){
            System.out.println(st.nextToken());
        }
        
    }
}


****************************************************************************************************

/*string class in java all constructer and methods */
class string_all{
	public static void main(String []args){
		//constructor uses
		String str1=new String();//public String();
		System.out.println(str1);
		
		String strr=new String("is the best college of Bihar");
		String str=new String("Bhagalpur College Of Engineering ");//public String(string);
		String str0=new String("Bhagalpur College Of Engineering ");//public String(string);
		String str00=new String("bhagalpur college Of Engineering");//public String(string);
		System.out.println(str);
		
		byte[] b={65,66,67,68,69,70};
		String str2=new String(b);//public String(byte[] b);
		System.out.println(str2);
		
		String str3=new String(b,2,4);//public String(byte[] b,int start_index,int no_of_elements)
		System.out.println(str3);
		
		char[] c={'A','B','C','D','E'};
		String str4=new String(c);//public String(char[] c);
		System.out.println(str4);
		
		String str5=new String(c,1,3);//public String(char[] c,int start_index,int no_of_element);
		System.out.println(str5);
	
	 //methods uses
		
		System.out.println(str.length());//public int length();
		
		System.out.println(str.concat(strr));//public String concat(String data);
		
		String st="bipin".concat("kumar").concat("sharma");
		System.out.println(st);
		
		System.out.println(str.equals(str0));//public boolean equals(String data);
		
		System.out.println(str0.equalsIgnoreCase(str00));//public bolean equalIgnoreCase(String data);
		
		System.out.println(str.compareTo(strr));//public int compareTo(String data);
		System.out.println(str.compareTo(str0));//public int compareTo(String data);
		
		System.out.println(str.startsWith("Bhagalpur"));//public boolean startsWith(String data);
		
		System.out.println(str.endsWith("Engineering "));//public boolean endsWith(String data);
		
		System.out.println(str.contains("College Of "));//public boolean contains(String data);
		
		System.out.println(strr.replace('i','I'));//public String replace(char old_char,char new_char);
		
		System.out.println(str.indexOf("Co"));//public int indexOf(String str);
		
		System.out.println(str.lastIndexOf("Co"));//public int lastIndexOf(String str);
			
		System.out.println(str.charAt(11));//public char charAt(int index);	
		
		System.out.println(str.substring(10));//public String substring(int start_index);

		System.out.println(str.substring(1,5));//public String substring(int start_index,int no_of_element);
		
		String[] s=str.split(" ");//public String[] split(String delimter);
		for(String s1:s){
		System.out.println("split"+s1);//for(int i=0;i<s.length();i++) 
		}
		
		byte[] b1=str.getBytes();//public byte[] getBytes();
		for(int i=0;i<b1.length;i++){
		System.out.println(b1[i]+"  "+(char)b1[i]);
		}
		
		char[] c1=str.toCharArray();//public char[] toCharArray();
		for(int i=0;i<c1.length;i++){
			System.out.println(c1[i]+"  ");
		} 
		
		String s1=new String(" Bhagalpur College Of Engineering ");
		System.out.println(s1.trim());//public String trim(); space remove begin and end 
		
		System.out.println(str.toLowerCase());//public String toLowerCase();
		
		System.out.println(str00.toUpperCase());//public String toUpperCase();
		
		
		
		
		System.out.println("         ******************STRINGBUFFER*********************              ");
		
		//StringBuffer constructure  
		
		StringBuffer sb=new StringBuffer();// public StringBuffer();
		StringBuffer sb0=new StringBuffer();// public StringBuffer();
		StringBuffer sb00=new StringBuffer();// public StringBuffer();
		
		System.out.println("the default capacity  :"+sb.capacity());
		
		StringBuffer sb1=new StringBuffer(10);//public StringBuffer(int capacity);
		
		System.out.println("the specified capacity :"+sb.capacity());
		
		StringBuffer sb2=new StringBuffer("bipin kumar sharma");// public StringBuffer(string data);
		StringBuffer sb3=new StringBuffer(" is work on hackerrank ");// public StringBuffer(string data);
		System.out.println(sb);
		
		
		//StringBuffer methods 
		
		System.out.println(sb2.append(sb3));//StringBuffer append(String str);
		System.out.println(sb2.append("is work on android "));//StringBuffer append(String str);
		
		
		sb.ensureCapacity(10);// public void ensureCapacity(int capacity);
		sb0.ensureCapacity(25);
		sb00.ensureCapacity(35);
		
		System.out.println(sb.capacity());
		System.out.println(sb0.capacity());
		System.out.println(sb00.capacity());


		System.out.println(sb2.reverse());// public StringBuffer reverse();
		
		System.out.println(sb2.insert(5," a big hacher in future "));//public StringBuffer insert(string data);
		
		System.out.println(sb2.delete(2,5));//public StringBuffer delete(int start_index,int end_index);
		
		String bipin=sb1.toString();//public String toString();
		System.out.println(bipin);
		System.out.println(sb1);
	}

}

*************************************************************************************************

/**************************  EXCEPTION HANDLING  *************************/
/*type of predefined exception */
class ArithmeticException{
public static void main(String []args){
int a=10,b=0;
float f=a/b;//ArithmeticException
System.out.println(f);
}
}


class NullPointerException{
	public static void main(String []args){
		java.util.Date d=null;//NullPointerException
		System.out.println(d);
	}
}







class A{
	static {
		System.out.println("class loading");
	}
}
class ClassNotFoundException{
	public static void main(String []args)throws Exception{
		Class c=Class.forName("AA");
	}

}





class inst{
	static{
		System.out.println("class loading");
	}
	inst(int i){                             //InstantiationException  not o-arg constructor 
		System.out.println("object creation");
	}
}
class InstantiationException{
	public static void main(String []args)throws Exception{
		Class c=Class.forName("inst");
		Object obj=c.newInstance();
	}

}






class illeg{
	static{
		System.out.println("class loading");
	}
	private illeg(){
		System.out.println("object created");    //IllegalAccessException   b'z private 
	}
}
class IllegalAccessException{
public static void main(String []args)throws Exception{
	Class c=Class.forName("illeg");
	Object obj=c.newInstance();
}
}



class cce1{
	}
	class cce2 extends cce1{
		
	}
class ClassCastException{
	public static void main(String []args){
		cce1 c1=new cce1();
		cce2 c2=(cce2)c1;  ///ClassCastException 
	}
}

*********************************THROW KEYWORD************************************

class throwkeyword{
public static void main(String []args)throws Exception{
	String sid=args[0];
	String sname=args[1];
	int smarks=Integer.parseInt(args[2]);
	System.out.println("student details");
	System.out.println("student id :"+sid);
	System.out.println("student name :"+sname);
	System.out.println("student marks :"+smarks);
	if(smarks >=0 && smarks <=100){
		System.out.println("student marks are valid ");
	}
	else{
		throw new RuntimeException("Invalid marks please enter student marks with in the range from 0 to 100");
	  //System.out.println("unrechable ");	//unreachable statement
	}
	
	
}
}




*****************************
import java.io.*;
class A{
	void add() throws Exception{
		concat();
	}
	void concat() throws IOException{
		throw new IOException("My IOException");
	}
}
class throws_keyword{
public static void main(String []args)throws Throwable{
	A a=new A();
	a.add();
	
}
}
*****************************


/* try-catch-finally block */
import java.io.*;

class try_catch_finally{
public static void main(String []args){
	try{
		int a=100;
		int b=0;
		float f=a/b;
		//generate exception in try block
	}catch(Exception e){
		e.printStackTrace();
		System.out.println();
		System.out.println(e);
		System.out.println();
		System.out.println(e.getMessage());
		
	}finally{
		
	}
	
	
}
}
*****************************
/* try_catch_finally*/
class try_catch_finally1{
public static void main(String []args){
	
	System.out.println("Before try ");
	try{
		System.out.println("inside try before excution");
	int a =100;
	int b=0;
	float f=a/b;
	System.out.println("inside try after excution");
	}
	catch(Exception e){
		System.out.println("inside catch");
		
	}
	finally{
		System.out.println("inside finally");
	}
	System.out.println("outside finally");
}
}
*****************************

/* try_catch_finally*/
class try_catch_finally2{
public static void main(String []args){
	
	System.out.println("Before try ");
	try{
		System.out.println("inside try ");
	
	
	}
	catch(Exception e){
		System.out.println("inside catch");
		
	}
	finally{
		System.out.println("inside finally");
	}
	System.out.println("outside finally");
}
}
******************************
class A{
int m1(){
try{
	return 10;
}
catch(Exception e){
	return 20;
}
finally{
	return 30;
}
}
}
class try_catch_finally3{
	public static void main(String []args){
		A a=new A();
		int val=a.m1();
		System.out.println(val);
	}
}
***************************

/*nested try_catch_block */

class A{
int m1(){
try{
	try{
		return 1;
	}catch(Exception e){
		return 2;
	}finally{
		return 3;
	}
	//return 10;    unreachable statement 
}
catch(Exception e){
	try{
		return 4;
	}catch(Exception e1){
		return 5;
	}finally{
		return 6;
	}
	//return 20;   unreachable statement
}
finally{
	try{
		return 7;
	}catch(Exception e){
		return 8;
	}finally{
		return 9;
	}
	//return 30;   unreachable statement 
}
}
}
class nested_try_catch_finally3{
	public static void main(String []args){
		A a=new A();
		int val=a.m1();
		System.out.println(val);
	}
}

**************************

/*user defined exception */
class InvalidMarkException extends Exception {
InvalidMarkException(String exception_msg){
	super(exception_msg);
}
}
class InvalidMarskException{
	public static void main(String[] args){
		try{
			throw new InvalidMarkException("MArks are invalid ,please enter the Marks with in the range from 0 to 100");
		}catch(InvalidMarkException e){
			e.printStackTrace();
		}
	}
}

**********************************


import java.io.*;
import java.util.*;
class  InsufficientFundException extends Exception{
InsufficientFundException(String err_msg){
super(err_msg);
}
}
class Transcation{
	String accNo,accName,accType;
	int initial_amt=2000;
	Transcation(String accNo,String accName,String accType){
		this.accNo=accNo;
		this.accName=accName;
		this.accType=accType;
		
	}
	public void withdrow(int wd_amt){
		try{
			System.out.println("Transcation Details :");
			System.out.println("Account Number : "+accNo);
			System.out.println("Account Name :"+accName);
			System.out.println("Account Type :"+accType);
			System.out.println("Transcation Status : withdrow ");
			System.out.println("withdrow amount :"+wd_amt);
			if(wd_amt<initial_amt){
				initial_amt=initial_amt-wd_amt;
			System.out.println("Total Amount :"+initial_amt);
			System.out.println("Transcation status : SUCCESS");
			}
			else{
				System.out.println("Total Amount:"+initial_amt);
				System.out.println("Transcation status: FAILURE");
				throw new InsufficientFundException("Funds are not sufficient in your account ,please enter the valid withdrow amount ");
				
			}
		}catch(InsufficientFundException e){
			System.out.println(e.getMessage());
		}finally{
			System.out.println("***********Thanq , visit again*******************");
		}
	}
}
class InsufficientFund{
	public static void main(String[] args){
		Transcation t1=new Transcation("3325001500099942","bipin kumar","saving");
		System.out.println("Enter withdraw amount ");
		Scanner s=new Scanner(System.in);
		int amt=s.nextInt();
		t1.withdrow(amt);
		
	}
}

**************************
**************************
**************************
**************************
/*  event handling  */


import java.awt.*;
import java.awt.event.*;
class MyWindowListener implements WindowListener{
	public void windowOpened(WindowEvent we){
		System.out.println("Window Opened");
		
	}
	public void windowClosing(WindowEvent we){
		System.out.println("window closing");
		System.exit(0);
	}
	public void windowClosed(WindowEvent we){
		System.out.println("window closed");
	}
	public void windowIconified (WindowEvent we){
		System.out.println("window Iconfied");
	}
	public void windowDeiconified(WindowEvent we){
		System.out.println("window deiconified");
	}
	public void windowActivated(WindowEvent we){
		System.out.println("window activated");
	}
	public void windowDeactivated(WindowEvent we){
		System.out.println("window deactivated");
	}
	
}
class MyFrame extends Frame{
	MyFrame(){
		this.setVisible(true);
		this.setSize(500,500);
		this.setTitle("window event example");
		this.setBackground(Color.blue);
		this.addWindowListener(new MyWindowListener());
	}
}
class MyWindowListnerEvent{
	public static void main(String[] args){
		MyFrame mf=new MyFrame();
	}
}

************************************************
import java.awt.*;
import java.awt.event.*;
class MyWindowsLisener1 extends WindowAdapter{
    public void windowClosing(WindowEvent we){
		System.out.println("window closing");
		System.exit(0);
	}
	
}
class MyFrame1 extends Frame{
	MyFrame1(){
		this.setVisible(true);
		this.setSize(500,400);
		this.setTitle("window event example 1");
		this.setBackground(Color.pink);
		this.addWindowListener(new MyWindowsLisener1());
	}
}
class MYWindowListenerEvent1{
	public static void main(String[] args){
		MyFrame1 mf=new MyFrame1();
	}
}
****************************************************
import java.awt.*;
import java.awt.event.*;
class MyFrame2 extends Frame{
     MyFrame2(){
	 this.setVisible(true);
	 this.setSize(500,500);
	 this.setTitle("windows event example 2");
	 this.setBackground(Color.pink);
	 this.addWindowListener(new WindowAdapter(){
	 public void windowClosing(WindowEvent we){
	 System.exit(0);
	 }
	 });
	 }
	 
}
class MyWindowListenerEvent2{
    public static void main(String[] args){
	MyFrame2 mf=new MyFrame2();
	}
}
************************************

import java.awt.*;
import java.awt.event.*;
class MyMouseListener implements MouseListener{
	public void mousePressed(MouseEvent me){
		System.out.println("moused pressed ["+me.getX()+","+me.getY()+"]");
	}
	public void mouseReleased(MouseEvent me){
		System.out.println("moused released ["+me.getX()+","+me.getY()+"]");
	}
	public void mouseClicked(MouseEvent me){
		System.out.println("moused clicked ["+me.getX()+","+me.getY()+"]");
	}
	public void mouseEntered(MouseEvent me){
		System.out.println("moused enter ["+me.getX()+","+me.getY()+"]");
	}
	public void mouseExited(MouseEvent me){
		System.out.println("moused exited ["+me.getX()+","+me.getY()+"]");
	}
}	
	class MyFrame3 extends Frame{
		MyFrame3(){
			this.setVisible(true);
			this.setSize(500,500);
			this.setTitle("mouse event example");
			this.setBackground(Color.pink);
			this.addWindowListener(new WindowAdapter(){
				public void windowClosing(WindowEvent we){
					System.exit(0);
				}
			});
		}
	}

class MyMouseListenerEvent{
	public static void main(String[] args){
		MyFrame3 mf=new MyFrame3();
	}
}
*************************************
/*adapter class use to eliminate unneccassory method()*/
import java.awt.*;
import java.awt.event.*;
class MyKeyListener implements KeyListener{
    public void keyPressed(KeyEvent ke){
	 System.out.println("key pressed ["+ke.getKeyChar()+"]");
	}
	public void keyReleased(KeyEvent ke){
	 System.out.println("key released ["+ke.getKeyChar()+"]");
	}
	public void keyTyped(KeyEvent ke){
	 System.out.println("key type ["+ke.getKeyChar()+"]");
	}
}
class MyFrame4 extends Frame{
    MyFrame4(){
	 this.setVisible(true);
	 this.setSize(500,500);
	 this.setTitle("key event example");
	 this.setBackground(Color.pink);
	 this.addWindowListener(new WindowAdapter(){
	   public void windowClosing(WindowEvent we){
	    System.exit(0);
	   }
	 });
	}
}
class MyKeyListenerEvent{
public static void main(String[] args){
   MyFrame4 mf=new MyFrame4();
}
}
*******************************************
/*button event */
import java.awt.*;
import java.awt.event.*;
class colorsFrame extends Frame implements ActionListener{
	Button b1,b2,b3;
	colorsFrame(){
	  this.setVisible(true);
	  this.setSize(500,600);
	  this.setTitle("Buttom example");
	  this.addWindowListener(new WindowAdapter(){
	  public void windowClosing(WindowEvent we){
	   System.exit(0);
	  }
	  });
	 this.setLayout(new FlowLayout());
	 b1=new Button("RED");
	 b2=new Button("GREAN");
	 b3=new Button("BLUE");
	 b1.setBackground(Color.red);
	 b2.setBackground(Color.green);
	 b3.setBackground(Color.blue);
	 b1.addActionListener(this);
	 b2.addActionListener(this);
	 b3.addActionListener(this);
	 this.add(b1);
	 this.add(b2);
	 this.add(b3);
	 
	}
	public void actionPerformed(ActionEvent ae){
	  String label=ae.getActionCommand();
	  if(label.equals("RED")){
	   this.setBackground(Color.red);
	  }
	  if(label.equals("GREAN")){
	   this.setBackground(Color.green);
	  }
	  if(label.equals("BLUE")){
	   this.setBackground(Color.blue);
	  }
	  
	}
}
class ButtomEventExample{
	public static void main(String[] args){
	colorsFrame frame=new colorsFrame();
	}
}
*********************************


 /* TextField and TextArea Example  */
import java.awt.*;
import java.awt.event.*;
class LoginFrame extends Frame implements ActionListener{
	Label l1,l2;
	TextField tf1,tf2;
	Button b1;
	String status="";
	LoginFrame(){
	  this.setVisible(true);
	  this.setSize(500,500);
	  this.setTitle("LoginFrame");
	  this.setBackground(Color.pink);
	  this.setLayout(new FlowLayout());
	  this.addWindowListener(new WindowAdapter(){
	   public void windowClosing(WindowEvent we){
	   System.exit(0);
	   }
	  });
	  l1=new Label("User Name");
	  l2=new Label("Password");
	  tf1=new TextField(20);
	  tf2=new TextField(20);
	  b1=new Button("Login");
	  b1.addActionListener(this);
	  this.add(l1);
	  this.add(l2);
	  this.add(tf1);
	  this.add(tf2);
	  this.add(b1);
	  
	}
	public void actionPerformed(ActionEvent ae){
	  String uname=tf1.getText();
	  String upwd=tf2.getText();
	  tf2.setText(" ");
	  if(uname.equals("bipin") && upwd.equals("bipin")){
	    status="valid user";
		
	  }else{
	   status="invalid user";
	  }
	 repaint();
	}
	public void paint(Graphics g){
	 Font f=new Font("aval",Font.BOLD,30);
	 g.setFont(f);
	 g.drawString("status="+status,100,300);
	}
} 
class TextFieldExample{
    public static void main(String[] args){
	  LoginFrame lf=new LoginFrame();
	} 
}
***********************************

import java.awt.*;
import java.awt.event.*;
class CalculatorFrame extends Frame implements ActionListener{
	Label l1,l2,l3;
	TextField tf1,tf2,tf3;
	Button b1,b2,b3,b4;
	CalculatorFrame(){
	  this.setVisible(true);
	  this.setSize(500,500);
	  this.setTitle("CalculatorFrame Example");
	  this.setBackground(Color.pink);
	  this.addWindowListener(new WindowAdapter(){
	   public void windowClosing(WindowEvent we){
	     System.exit(0);
	   }
	  });
	  this.setLayout(null);
	  l1=new Label("first value");
	  l2=new Label("second value");
	  l3=new Label("result value");
	  tf1=new TextField(15);
	  tf2=new TextField(15);
	  tf3=new TextField(15);
	  b1=new Button("ADD");
	  b2=new Button("SUB");
	  b3=new Button("MUL");
	  b4=new Button("DIV");
	  b1.addActionListener(this);
	  b2.addActionListener(this);
	  b3.addActionListener(this);
	  //b4.addActionListener(this);
	  l1.setBounds(50,100,100,20);
	  l2.setBounds(50,130,100,20);
	  l3.setBounds(50,160,100,30);
	  tf1.setBounds(150,100,100,20);
	  tf2.setBounds(150,130,100,20);
	  tf3.setBounds(150,160,100,20);
	  b1.setBounds(50,220,50,30);
	  b2.setBounds(100,220,50,30);
	  b3.setBounds(150,220,50,30);
	  //b4.setBounds(150,220,50,30);
	  this.add(l1);this.add(l2);this.add(l3);
	  this.add(tf1);this.add(tf2);this.add(tf3);
	  this.add(b1);this.add(b2);this.add(b3);this.add(b4);
	  }
	  public void actionPerformed(ActionEvent ae){
	   try{
	    int fval=Integer.parseInt(tf1.getText());
	    int sval=Integer.parseInt(tf2.getText());
	    String button_label=ae.getActionCommand();
		if(button_label.equals("ADD")){
		 tf3.setText(" "+(fval+sval));
		}
		if(button_label.equals("SUB")){
		 tf3.setText(" "+(fval-sval));
		}
		if(button_label.equals("MUL")){
		 tf3.setText(" "+(fval*sval));
		}
		
		
		
	   }catch(Exception e){
	    e.printStackTrace();
	   }
	  }
	
}
class CalculatorFrameExample{
	public static void main(String[] args){
	 CalculatorFrame cf= new CalculatorFrame();
	} 
	}

************************************************


/*check box and radio button example */
import java.awt.*;
import java.awt.event.*;
class CheckRadioBox extends Frame implements ItemListener{
	Label l1,l2;
	Checkbox cb1,cb2,cb3,cb4,cb5;
	CheckboxGroup cbg;
	String qual="",gender="";
	CheckRadioBox(){
		this.setVisible(true);
		this.setSize(500,500);
		this.setTitle("CheckRadioButton Example");
		this.setLayout(new FlowLayout());
		this.setBackground(Color.pink);
		this.addWindowListener(new WindowAdapter(){
			public void windowClosing(WindowEvent we){
				System.exit(0);
			}
		});
		l1=new Label("Qualifications");
		l2=new Label("Gender");
		cb1=new Checkbox("B.Tech",null,false);
		cb2=new Checkbox("M.Tech",null,false);
		cb3=new Checkbox("P.H.D",null,false);
		cbg=new CheckboxGroup();
		cb4=new Checkbox("Male",cbg,false);
		cb5=new Checkbox("Female",cbg,false);
		cb1.addItemListener(this);
		cb2.addItemListener(this);
		cb3.addItemListener(this);
		cb4.addItemListener(this);
		cb5.addItemListener(this);
		this.add(l1);this.add(l2);this.add(cb1);
		this.add(cb2);this.add(cb3);this.add(cb4);this.add(cb5);
		
	}
	public void itemStateChanged(ItemEvent ie){
		if(cb1.getState()==true){
			qual=qual+cb1.getLabel()+" ";
		} 
		if(cb2.getState()==true){
			qual=qual+cb2.getLabel()+" ";
		} 
		if(cb3.getState()==true){
			qual=qual+cb3.getLabel()+" ";
		} 
		if(cb4.getState()==true){
			gender=cb4.getLabel()+" ";
		} 
		if(cb5.getState()==true){
			gender=cb5.getLabel()+" ";
		} 
		repaint();
	}
	public void paint(Graphics g){
		Font f=new Font("qual",Font.BOLD,25);
		g.setFont(f);
		g.drawString("Qualifications :"+qual,50,200);
		g.drawString("Gender :"+gender,50,250);
		qual=" ";
	}
}
class CheckRadioBoxExample{
	public static void main(String[] args){
		CheckRadioBox cb=new CheckRadioBox();
	}
}

*************************************


/* Example of List and Choice */
import java.awt.*;
import java.awt.event.*;
class ListChoiceFrame extends Frame implements ItemListener{
    Label l1,l2;
	List l;
	Choice ch;
	String tech="";
	String prof="";
	ListChoiceFrame(){
	    this.setVisible(true);
		this.setSize(500,500);
		this.setTitle("ListChoiceFrame Example");
		this.setLayout(new FlowLayout());
		this.setBackground(Color.pink);
		this.addWindowListener(new WindowAdapter(){
			public void windowClosing(WindowEvent we){
				System.exit(0);
			}
		});
		l1=new Label("Technology");
		l2=new Label("Profession");
		l=new List(4,true);
		l.add("c");l.add("c++");l.add("java");l.add(".net");
		l.add("oracle");l.add("android");
		ch=new Choice();
		ch.add("Student");ch.add("Employee");ch.add("Teacher");
		ch.add("Business");
		l.addItemListener(this);
		ch.addItemListener(this);
		this.add(l1);this.add(l2);this.add(l);this.add(ch);
		
		
	}
	public void itemStateChanged(ItemEvent ie){
	  String[] item=l.getSelectedItems();
	  for(int i=0;i<item.length;i++){
	   tech=tech+item[i]+" ";
	  }
	  prof=ch.getSelectedItem();
	  repaint();
	}
	public void paint(Graphics g){
	 Font f=new Font("arial",Font.BOLD,25);
	 g.setFont(f);
	 g.drawString("Technology :"+tech,50,200);
	 g.drawString("Profession :"+prof,50,150);
	 tech=" ";
	 
	}
	
}
class ListChoiceFrameExample{
   public static void main(String[] args){
     ListChoiceFrame lc=new ListChoiceFrame();
   }
   }

***************************************

/* MenuBar,Menu,MenuItem Example */
import java.awt.*;
import java.awt.event.*;
class MenuFrame extends Frame implements ActionListener{
	MenuBar mb;
	Menu m;
	MenuItem mi1,mi2,mi3,mi4;
	String item="";
	MenuFrame(){
		this.setVisible(true);
		this.setSize(500,500);
		this.setTitle("MenuDetailsExample");
		this.setBackground(Color.pink);
		this.addWindowListener(new WindowAdapter(){
			public void windowClosing(WindowEvent we){
				System.exit(0);
			}
		});
		mb=new MenuBar();
		this.setMenuBar(mb);
		m=new Menu("File");
		mb.add(m);
		mi1=new MenuItem("New");
		mi2=new MenuItem("open");
		mi3=new MenuItem("save");
		mi4=new MenuItem("save is");
		m.add(mi1);m.add(mi2);m.add(mi3);m.add(mi4);
		mi1.addActionListener(this);
		mi2.addActionListener(this);
		mi3.addActionListener(this);
		mi4.addActionListener(this);
	}
	public void actionPerformed(ActionEvent ae){
		item=ae.getActionCommand();
		repaint();
		
	}
	public void paint(Graphics g){
		Font f=new Font("arial",Font.BOLD,25);
		g.setFont(f);
		g.drawString("Selected Item :"+item,50,200);
	}
	
}
class MenuDetailsExample{
	public static void main(String[] args){
		MenuFrame mf=new MenuFrame();
	}
// not perfect run 

*********************************************
   
**********************RELATIONSHIP IN JAVA ***********************

/* one to one relation ship */
class Account{
	String accNo,accName,accType;
	Account(String accNo,String accName,String accType){
		this.accNo=accNo;
		this.accName=accName;
		this.accType=accType;
	}
}
class Employee{
	String eid;
	String ename;
	float esal;
	String eaddr;
	Account acc;
	Employee(String eid,String ename,float esal,String eaddr,Account acc ){
		this.eid=eid;
		this.ename=ename;
		this.esal=esal;
		this.eaddr=eaddr;
		this.acc=acc;
		
	}
	public void getEmpDetails(){
		System.out.println("Employee Details :");
		System.out.println("Employee id :"+eid);
		System.out.println("Employee name :"+ename);
		System.out.println("Employee salary :"+esal);
		System.out.println("Employee address :"+esal);
		System.out.println("Account Details :");
		System.out.println("Account number :"+acc.accNo);
		System.out.println("Account name :"+acc.accName);
		System.out.println("Account type :"+acc.accType);
		
	}
}
class oneToOneAssociation{
	public static void main(String[] args){
		Account acc=new Account("3325001500099942","bipin kumar","saving");
		Employee emp =new Employee("E-111","bipin",15000.0f,"bgp",acc);
		emp.getEmpDetails();
	}
}
**************************************
/*one to meny association */
class Employees{
	String eid,ename,eaddr;
	float esal;
	Employees(String eid,String ename,float esal,String eaddr){
		this.eid=eid;
		this.ename=ename;
		this.esal=esal;
		this.eaddr=eaddr;
	}
}
class Department{
	String did,dname;
	Employees[] emps;
	Department(String did,String dname,Employees[] emps){
		this.did=did;
		this.dname=dname;
		this.emps=emps;
		
	}
	public void getDeptDetails(){
		System.out.println("Department Details");
		System.out.println("Department id :"+did);
		System.out.println("Department name :"+dname);
		System.out.println("Employees Details ");
		System.out.println("EID\tENAME\tESAL\tEADDRESS");
		
		for(int i=0;i<emps.length;i++){
			Employees e=emps[i];
			System.out.println(e.eid+"\t"+e.ename+"\t"+e.esal+"\t"+e.eaddr);
		}
	}
}
class oneToMenyAssociation{
	public static void main(String[] args){
		Employees e1=new Employees("E-111","bipin",10000,"bgp");
		Employees e2=new Employees("E-222","kumar",20000,"bgp");
		Employees e3=new Employees("E-333","sharma",30000,"bgp");
		Employees e4=new Employees("E-444","bipin",40000,"bgp");
		Employees[] emps={e1,e2,e3,e4};
		Department dept=new Department("D-111","science",emps);
		dept.getDeptDetails();
	}
}
****************************************
/* meny to one association */
class Branch{
	String bid,bname;
	Branch(String bid,String bname){
		this.bid=bid;
		this.bname=bname;
	}
}
class Student{
	String sid,sname,saddr;
	Branch branch;
	Student(String sid,String sname,String saddr,Branch branch){
		this.sid=sid;
		this.sname=sname;
		this.saddr=saddr;
		this.branch=branch;
	}
	public void getStudentDetails(){
		System.out.println("Student Details ");
		System.out.println("Student id :"+sid);
		System.out.println("Student name :"+sname);
		System.out.println("Student address :"+saddr);
		System.out.println("Branch id :"+branch.bid);
		System.out.println("Branch name :"+branch.bname);
		
	}
}
class menyToOneAssociation{
	public static void main(String[] args){
		Branch branch=new Branch("B-111","cs");
		Student s1=new Student("s-111","bipin","bgp",branch);
		Student s2=new Student("s-112","kumar","bgp",branch);
		Student s3=new Student("s-113","sharma","bgp",branch);
		Student s4=new Student("s-114","bipin","bgp",branch);
	    s1.getStudentDetails();
		System.out.println();
	    s2.getStudentDetails();
		System.out.println();
	    s3.getStudentDetails();
		System.out.println();
	    s4.getStudentDetails();
	}
}

***************************************
/*meny to meny association */
class course{
	String cid,cname;
	int ccost;
	course(String cid,String cname,int ccost){
		this.cid=cid;
		this.cname=cname;
		this.ccost=ccost;
	}
}
class Students{
	String sid,sname,saddr;
	course[] crs;
	Students(String sid,String sname,String saddr ,course[] crs){
		this.sid=sid;
		this.sname=sname;
		this.saddr=saddr;
		this.crs=crs;
	}
	public void getStudentDetails(){
		System.out.println("Student Details");
		System.out.println("Student id :"+sid);
		System.out.println("Student name :"+sname);
		System.out.println("Student Address :"+saddr);
		System.out.println("CID\tCNAME\tCCOST");
		for(int i=0;i<crs.length;i++){
			course c=crs[i];
			System.out.println(c.cid+"\t"+c.cname+"\t"+c.ccost);
		}
		System.out.println();
	}
}
class menyToMenyAssociation{
	public static void main(String[] args){
		course c1=new course("c-111","c",1000);
		course c2=new course("c-112","c++",2000);
		course c3=new course("c-113",".net",3000);
		course c4=new course("c-114","java",4000);
		course[] crs={c1,c2,c3,c4};
		Students s1=new Students("s-111","bipin","bgp",crs);
		Students s2=new Students("s-112","kumar","bgp",crs);
		Students s3=new Students("s-113","sharma","bgp",crs);
		Students s4=new Students("s-114","bipin","bgp",crs);
		s1.getStudentDetails();
		s2.getStudentDetails();
		s3.getStudentDetails();
		s4.getStudentDetails();
	}
}
****************************************
   /* inheritence in java */
class Employees{
   String eid,ename,eaddr;
   float esal;
   public void getEmpDetails(){
      System.out.println("Employee id :"+eid);
	  System.out.println("Employee name :"+ename);
	  System.out.println("Employee salary :"+esal);
	  System.out.println("Employee address :"+eaddr);
	  
   }
}
class Manager extends Employees{
	Manager(String eid1,String ename1,float esal1,String eaddr1){
	   eid=eid1;
	   ename=ename1;
	   esal=esal1;
	   eaddr=eaddr1;
	   
	}
	public void getManagerDetails(){
	   System.out.println("Manger Details");
	   getEmpDetails();
	}
}
class Accountant extends Employees{
	Accountant(String eid1,String ename1,float esal1,String eaddr1){
	   eid=eid1;
	   ename=ename1;
	   esal=esal1;
	   eaddr=eaddr1;
	}
	public void getAccountDetails(){
	   System.out.println("Accountant Details ");
	   getEmpDetails();
	}
}
class Inheritance{
public static void main(String[] args){
  Manager m=new Manager("E-111","bipin kumar",50000.0f,"bhagalpur");
  m.getManagerDetails();
  System.out.println();
  Accountant ac=new Accountant("E-222","bipin sharma",40000.0f,"gaya");
  ac.getAccountDetails();
}
}

**************************************

/*static  keyword in inheritance */
class A{
 static{
   System.out.println("SB-A");
 }
}
class B extends A{
   static{
   System.out.println("SB-B");
   }
}
class C extends B{ 
   static{
   System.out.println("SB-C");
   }
}
class staticKey1{
  public static void main(String[] args){
    C c=new C();
  }
}

************************************

class A{
  static int m1(){
	  System.out.println("m1-A");
	  return 10;
  }
  static{
	  System.out.println("SB-A");
  }
  static int i=m1();
}
class B extends A{
	static int j=m2();
	static{
		System.out.println("SB-B");
	}
	static int m2(){
		System.out.println("m2-B");
		return 20;
	}
}
class C extends B{
	static{
		System.out.println("SB-C");
	}
	static int k=m3();
	static int m3(){
		System.out.println("m3-C");
		return 30;
	}
}
class staticKey2{
	public static void main(String[] args){
		C c1=new C();
		System.out.println();
		C c2=new C();
		System.out.println("c2 not perform b'z code r already loading in memory dua to static ");
	}
}

***********************************

/*instance in inheritance */
class A{
	A(){
		System.out.println("A-con");
	}
}
class B extends A{
	B(){
		System.out.println("B-con");
	}
}
class C extends B{
	C(){
		System.out.println("C-con");
	}
}
class InstanceInInheritance{
	public static void main(String[] args){
		C c=new C();
	}
}

***************************************

class A{
	A(){
		System.out.println("A-con");
	}
	{
		System.out.println("IB-A");
	}
	int m1(){
		System.out.println("m1-A");
		return 1;
	}
	int i=m1();
}
class B extends A{
	{
		System.out.println("IB-B");
	}
	int j=m2();
	int m2(){
		System.out.println("m2-B");
		return 2;
	}
	B(){
		System.out.println("B-con");
	}
}
class C extends B{
	C(){
		System.out.println("C-con");
	}
	int m3(){
		System.out.println("m3-C");
		return 3;
	}
	{
		System.out.println("IB-C");
	}
	int k=m3();
}
class InstanceInInheritance1{
	public static void main(String[] args){
		C c=new C();
	}
}

*******************************

/*static and instance in inheritance */
class A{
    A(){//constructor
		System.out.println("A-con");
	}
    static{//static block
		System.out.println("SB-A");
	}    
	int m1(){//instance method 
		System.out.println("IM-A");
		return 1;
	}
	static int i=m2();
	{           //instance block
	System.out.println("IB-A");
	}
	int j=m1();
	static int m2(){//static method
		System.out.println("SM-A");
		return 3;
	}
	
}
class B extends A{
	B(){
		System.out.println("B-con");
	}
	{
		System.out.println("IB-B");
	}
	static{
		System.out.println("SB-B");
	}
	int m3(){
		System.out.println("IM-B");
		return 5;
	}
	static int m4(){
		System.out.println("SM-B");
		return 6;
	}
	int k=m3();
	static int l=m4();
}
class C extends B{
	static {
		System.out.println("SB-C");
	}
	static int m5(){
		System.out.println("SM-C");
		return 4;
	}
	static int m=m5();
	C(){
		System.out.println("C-con");
	}
	{
		System.out.println("IB-C");
	}
	int m6(){
		System.out.println("IM-C");
		return 5;
	}
	int n=m6();
}
class staticInstance{
	public static void main(String[] args){
		C c1=new C();
		System.out.println();
		C c2=new C();
	}
}
/*all static blocks and methods first excute then instance block and methods are excuted with respective constructor in inheritance */

*****************************************
/* super keyword in inheritance */
 /* super class variable */
 
class A{
	int i=10,j=20;
}
class B extends A{
	int i=12,j=22;
	B(int i,int j){
		System.out.println(i+" "+j);//local variable
		System.out.println(this.i+" "+this.j);//current class variable
		System.out.println(super.i+" "+super.j);//super class variable
	}
}
class superVariable{
	public static void main(String[] args){
		B b=new B(30,40);
	}
}

**********************************

/* super class method **/
class A{
	void m1(){
		System.out.println("m1-A");
	}
}
class B extends A{
	void m2(){
		System.out.println("m2-B");
		m1();//current class method
		this.m1();//current class method
		super.m1();//super class method
	}
	void m1(){
		System.out.println("m1-B");
	}
}
class superMethod{
	public static void main(String[] args){
		B b=new B();
		b.m2();
	}
}

***************************************

/* super class constructor */
class A{
	A(){
		System.out.println("A-con");
	} //*/
	A(int i){
		System.out.println("A-param-int con");
	}
}
class B extends A{
	B(){
		super(10);//1st statement in cons not in method
		//super();// not more than one super keyword 
		System.out.println("B-con");
	}
/*	void m1(){
		super(10);//not call in method 
		System.out.println("m1_b");
	}*/
}
class superConstructor{
	public static void main(String[] args){
		B b=new B();
	}
}

******************************


/* super 0 arg constructor  */
class A{
	A(){
		System.out.println("A-con");
	}
}
class B extends A{ 
	//B(int i){
	B(){
		System.out.println("B-con");
	}
}
class C extends B{
	C(){
	//	super(10);  for param cons 
	System.out.println("C-con");
}
}
class superZeroConstructore{
	superZeroConstructore(){
		super();
	}
	public static void main(String[] args){
		C c=new C();
	}
}

*******************************

/* class level type casting in inheritance */
class A{
	void m1(){
		System.out.println("m1-A");
	}
}
class B extends A{
	void m2(){
		System.out.println("m2-B");
	}
}
class upCasting{
	public static void main(String[] args){
		B b=new B();
		b.m1();
		b.m2();
		System.out.println();
		
		A a=b;
		a.m1();
		//a.m2();     //cannot find m2() in A 
		System.out.println();
		
		A a1=new B();
		a1.m1();
		//a2.m2();    //cannot find m2() in A 
		
		A a2=new A();
		a2.m1();
		//a2.m2();
	}
}

*******************************

/* down casting */
class A{
	void m1(){
		System.out.println("m1-A");
	}
}
class B extends A{
	 void m2(){
		 System.out.println("m2-B");
	 }
}
class downCasting{
	public static void main(String[] args){
	/*	A a=new A();
		B b=a;     ///error
		b.m1();
		b.m2();*/
		
	/*	A a1= new A();
		B b1= (B)a1;  //Exception given 
		
		b1.m1();
		b1.m2();    */
		
		A a2=new B();
		B b2=(B)a2;
		b2.m1();
		b2.m2();
		
		
	}
}
**************************************

/* down casting type in inheritance */
class A{}
class B extends A{}
class C extends B{}
class D extends C{}
class downCastingType{
	public static void main(String[] args){
	/*	A a=new A();
		B b=a;  //incompatible types
	*/
	/*    A a=new A();
		B b=(B)a;//ClassCastException
	*/
	/*	A a=new D();
		D d=(D)a ;  // NO ERROR  NO EXCEPTION
	*/
	/*	A a=new D();
		C d=(D)a ;   //NO ERROR  NO EXCEPTION
	*/
	/*	A a=new B();
		C d=(C)a ;  // EXCEPTION 
	*/
	/*	A a=new C();
		B d=(D)a ;   //EXCEPTION
	*/
	/*	A a=new D();
		B d=(C)a ;    //NO ERROR  NO EXCEPTION
	*/
		A a=new D();
		D d=(D)(C)(B)a ; //NO ERROR NO EXCEPTION
	
	
	}
}

*****************************



**********************************
****************TUTORIAL POINT EXAMPLE **************

//package com.tutorialspoint.gui;

import java.awt.*;
import java.awt.event.*;

public class AwtControlDemoLabel {

   private Frame mainFrame;
   private Label headerLabel;
   private Label statusLabel;
   private Panel controlPanel;

   public AwtControlDemoLabel(){
      prepareGUI();
   }

   public static void main(String[] args){
      AwtControlDemoLabel  a = new AwtControlDemoLabel();
      a.showLabelDemo();
   }

   private void prepareGUI(){
      mainFrame = new Frame("Java AWT Examples");
      mainFrame.setSize(400,400);
      mainFrame.setLayout(new GridLayout(3, 1));
      mainFrame.addWindowListener(new WindowAdapter() {
         public void windowClosing(WindowEvent windowEvent){
            System.exit(0);
         }        
      });    
      headerLabel = new Label();
      headerLabel.setAlignment(Label.CENTER);
      statusLabel = new Label();        
      statusLabel.setAlignment(Label.CENTER);
      statusLabel.setSize(350,100);

      controlPanel = new Panel();
      controlPanel.setLayout(new FlowLayout());

      mainFrame.add(headerLabel);
      mainFrame.add(controlPanel);
      mainFrame.add(statusLabel);
      mainFrame.setVisible(true);  
   }

   private void showLabelDemo(){
      headerLabel.setText("Control in action: Label");      

      Label label = new Label();
      label.setText("Welcome to TutorialsPoint AWT Tutorial.");
      label.setAlignment(Label.CENTER);
      label.setBackground(Color.BLUE);
      label.setForeground(Color.RED);
      controlPanel.add(label);
   
      mainFrame.setVisible(true);  
   }
}
**************************************** 

/*HAS-A relation ship  */
class AccountHas{
	String accNo,accType,accName;
	int bal;
	public AccountHas(String accNo,String accName,String accType ,int bal){
		this.accNo=accNo;
		this.accName=accName;
		this.accType=accType;
		this.bal=bal;
		
	}
}
class TranscationHas{
	public void withdrowHas(AccountHas acc,int wd_amt){
		acc.bal=acc.bal-wd_amt;
		System.out.println("Transcation Details");
		System.out.println("Account number :"+acc.accNo);
		System.out.println("Account name :"+acc.accName);
		System.out.println("Account Type :"+acc.accType);
		System.out.println("Withdrawal Amount :"+wd_amt);
		System.out.println("Total Amount :"+acc.bal);
		System.out.println("SUCCESS");
	}
}
class hasARelationship{
	public static void main(String[] args){
		AccountHas acc= new  AccountHas("3325001500099942","bipin kumar","saving",2000);
		TranscationHas ts =new TranscationHas();
		ts.withdrowHas(acc,1000);
		
	}
}
****************************************

/*polymorphism in java*/
/* method overloading */
class A{
	void add(int i,int j){
		int k=i+j;
		System.out.println(k);
	}
	void add(float f1,float f2){
		float f3=f1+f2;
		System.out.println(f3);
	}
	void add(String s1,String s2){
		String s=s1+s2;
		System.out.println(s);
	}
}
class methodOverloading{
	public static void main(String[] args){
		A a=new A();
		a.add(10,20);
		a.add(10.05f,20.05f);
		a.add("bipin","kumar");
	}
}

***************************************

/* methos overriding */
class A{
	void m1(){
		System.out.println("m1-A");
	}
}
class B extends A{
	void m1(){
		System.out.println("m1-B");
	}
}
class methodOverriding{
	public static void main(String[] args){
		A a=new A();
		a.m1();//m1-A o/p
		// status -: method Overriding req sub class object
		B b=new B();
		b.m1();// m1-B both o/p 
		//status :- 
		
		A a1=new B();
		a1.m1();// m1-B   overriding performed 
	}
}
*****************************
/* method overriding */
class Loan{
	public float getIR(){
		return 5.0f;
	}
}
class Craft_Loan extends Loan{
	public float getIR(){
		return 10.0f;
	}
}
class Study_Loan extends Loan{
	public float getIR(){
		return 15.0f;
	}
}
class Gold_Loan extends Loan{
	
}
class methodOverriding1{
	public static void main(String[] args){
		Loan cl=new Craft_Loan();
		System.out.println(cl.getIR());
	    Loan sl=new Study_Loan();
		System.out.println(sl.getIR());
		Loan gl=new Gold_Loan();
		System.out.println(gl.getIR());
	}
}
****************************************

/*method overriding rule */
Rule .1 .....................
class A{
	private void m1(){    //not private 
		System.out .println("m1-A");
	}
}   
class B extends A{
	void m1(){
		System.out.println("m1-B");
	}
}
class methodOverridingRule{
	public static void main(String[] args){
		A a=new A();
		a.m1();
	}
}     

Rule .2....................
/*method overriding rule */

class A{
//1.        private void m1(){    //not private 
//2.		void m1(){
//3.		final void m1(){	  // not final 
//4.    	void m1(){
//5.		final void m1(){
//6.		void m1(){
//7.		static void m1(){
//8.        static void m1(){  // no error but no overriding but overhiding
//9.   	    public void m1(){
	 
	 
	  
	  System.out .println("m1-A");
	}
}   
class B extends A{
//1.	void m1(){
//2.    int m1(){	     //return type same as super class method 
//3.	void m1(){	
//4.	final void m1(){  // no error
//5.    final void m1(){  // not both final 
//6.	private void m1(){  // not strong privileges than super
//7.	void static m1(){   // not static in super/sub class
//8.	static void m1(){
//9. 	void m1(){         // not less than scop of super class
		
		System.out.println("m1-B");
	}
}
class methodOverridingRule{
	public static void main(String[] args){
		A a=new A();
		a.m1();
	}
}   

********************************


/* abstract keyword in inhrotance */

/* abstract keyword */ 
abstract class A{
	void m1(){
		System.out.println("M1-A");
	}
	abstract void m2();
	abstract void m3();
}
class B extends A{
	void m2(){
		System.out.println("m2-B");
	}
	void m3(){
		System.out.println("m3-B");
		
	}
	void m4(){
		System.out.println("m4-B");
	}
}
class abstractClass{
	public static void main(String[] args){
	//	A a=new A();  cannot create object of abstract class 
	    A a=new B();
		a.m1();
		a.m2();
		a.m3();
	//	a.m4();      a not access this,b'z m4() not in A 
	   
	   B b=new B();
	   b.m1();
	   b.m2();
	   b.m3();
	   b.m4();
	}
}

***********************************************

/* abstract method implementation */
abstract class A{
	abstract void m1();
	abstract void m2();
	abstract void m3();
}
abstract class B extends A{
	void m1(){
		System.out.println("m1-B");
	}
}
class C extends B{
	void m2(){
		System.out.println("m2-C");
	}
	void m3(){
		System.out.println("m3-C");
	}
}
class abstractImplementation{
	public static void main(String[] args){
		A a=new C();
		a.m1();
		a.m2();
		a.m3();
	}
}
*******************************


/* abstract class and concreate class extends */
class A{
	void m1(){
		System.out.println("m1-A");
	}
}
abstract class B extends A{
	abstract void m2();
	abstract void m3();
	
}
class C extends B{
	void m2(){
		System.out.println("m2-C");
		
	}
	void m3(){
		System.out.println("m3-C");
	}
	void m4(){
		System.out.println("m4-C");
	}
}
class abstractConcreteExtends{
	public static void main(String[] args){
		A a=new A();
		a.m1();
		System.out.println();
		
		B b=new C();
		b.m1();
		b.m2();
		b.m3();
		System.out.println();
		C c=new C();
		c.m1();
		c.m2();
		c.m3();
		c.m4();
	}
}

*******************************

/* abstract class constructor */
abstract class A{
	A(){
		System.out.println("A-con");
	}
}
class B extends A{
	B(){
		System.out.println("B-con");
	}
}
class abstractConstructor{
	public static void main(String[] args){
		B b=new B();
	}
}

**********************************

/* interface in inheritance */
interface I{
    int x=10;
	void m1();
	void m2();
	void m3();
}
class A implements I{
	public void m1(){
		System.out.println("m1-A");
	}
	public void m2(){
		System.out.println("m2-A");
	}
	public void m3(){
		System.out.println("m3-A");
	}
	public void m4(){
		System.out.println("m4-A");
	}
}
class interfaceExample{
	public static void main(String[] args){
		System.out.println(I.x);
		I i=new A();
		System.out.println(i.x);
		i.m1();
		i.m2();
		i.m3();
		
		A a=new A();
		System.out.println(A.x);
		System.out.println(a.x);
		a.m1();
		a.m2();
		a.m3();
		a.m4();
	}
}

************************************
/* multiple interface in inheritance */
interface I1{
	void m1();
}
interface I2{
	void m2();
}
interface I3{
	void m3();
}
class A implements I1,I2,I3{
	public void m1(){
		System.out.println("m1-A");
	}
	public void m2(){
		System.out.println("m2-A");
	}
	public void m3(){
		System.out.println("m3-A");
	}
}
class multiInterface{
	public static void main(String[] args){
		I1 i1=new A();
		i1.m1();
		System.out.println();
		I2 i2=new A();
		i2.m2();
		System.out.println();
		I3 i3=new A();
		i3.m3();
		
		A a=new A();
		a.m1();
		a.m2();
		a.m3();
	}
}

******************************
/* java 8 feature in interface */ 
/* 1. static method in interface */
interface I {
	void m1();
	void m2();
	static void m3(){
		System.out.println("static method in interface");
	}
}
class A implements I{
	public void m1(){
		System.out.println("m1-A");
	}
	public void m2(){
		System.out.println("m2-A");
	}
}
class staticInInterface{
	public static void main(String[] args){
		I i=new A();
		i.m1();
		i.m2();
		//i.m3();  not access static method by reference var
		I.m3();
	//	A.m3();    not acess 
	A a=new A();
	//  a.m3();    not access
	    a.m1();
	
	}
}
******************************

/* java 8 feature in interface */ 
/* default method in interface */
interface DB_Driver{
	default void getDriverClass(){
		System.out.println("sun.jdbc.odbc.JdbcOdbcDriver");
	}
	default void getDriverURL(){
		System.out.println("jdbc:odbc:dsn_name");
	}
}
class oracleDriver implements DB_Driver{
	public void getDriverClass(){
		System.out.println("oracle.jdbc.oracleDriver");
	}
	public void getDriverURL(){
		System.out.println("jdbc:oracle:thin@Localhost:1521:XE");
	}
}
class MySqlDriver implements DB_Driver{
	public void getDriverClass(){
		System.out.println("com.mysql.jdbc.Driver");
	}
	public void getDriverURL(){
		System.out.println("jdbc:mysql://Localhost:3306/db");
	}
}
class MsAccessDriver implements DB_Driver{
}
class defaultInInInterface{
	public static void main(String[] args){
	DB_Driver oracle_Driver=new oracleDriver();
	oracle_Driver.getDriverClass();
	oracle_Driver.getDriverURL();
	System.out.println();
	
	DB_Driver mysql_Driver=new MySqlDriver();
	mysql_Driver.getDriverClass();
	mysql_Driver.getDriverURL();
	System.out.println();
	
	DB_Driver msaccess_Driver=new MsAccessDriver();
	msaccess_Driver.getDriverClass();
	msaccess_Driver.getDriverURL();
	
	}
}

**************************************

/* object cloning == duplicate object create */
class EmpClone implements Cloneable{
	String eid,ename,eaddr;
	float esal;
	EmpClone(String eid,String ename ,float esal,String eaddr){
		this.eid=eid;
		this.ename=ename;
		this.esal=esal;
		this.eaddr=eaddr;
	}
	public void getEmpDetails(){
		System.out.println("Employee Details");
	    System.out.println("Employee id :"+eid);
		System.out.println("Employee name :"+ename);
		System.out.println("Employee sal :"+esal);
		System.out.println("Employee address :"+eaddr);
	}
	public Object clone()throws CloneNotSupportedException {
		Object obj=super.clone();
		return obj;
	}
}
class objectCloning{
	public static void main(String[] args)throws Exception{
		EmpClone e1=new EmpClone("E-111","bipin",1000.0f,"bgp");
		e1.getEmpDetails();
		System.out.println("original emp object ref"+e1);
		EmpClone e2=(EmpClone)e1.clone();
		System.out.println();
		System.out.println("Employee Details from duplicate object");
		e2.getEmpDetails();
		System.out.println("Duplicate Emp object "+e2);
		
	}
}

*****************************


/* shallow cloning */
class course{
	String cid,cname;
	int ccost;
	course(String cid,String cname,int ccost){
		this.cid=cid;
		this.cname=cname;
		this.ccost=ccost;
	}
}
class student implements Cloneable{
	String sid,sname,saddr;
	course crs;
	student(String sid,String sname,String saddr,course crs){
		this.sid=sid;
		this.sname=sname;
		this.saddr=saddr;
		this.crs=crs;
	}
	public void getStudentDetails(){
		System.out.println("student Details");
		System.out.println("student id :"+sid);
		System.out.println("student name :"+sname);
		System.out.println("student saddr :"+saddr);
		System.out.println("course Details");
		System.out.println("course id :"+crs.cid);
		System.out.println("course name :"+crs.cname);
		System.out.println("course cost :"+crs.ccost);
	}
	public Object clone() throws CloneNotSupportedException{
		Object obj=super.clone();
		return obj;
	}
	
}
class shallowCloning {
	public static void main(String[] args)throws Exception{
		course crs=new course("c-111","java",1000);
		student s1=new student("s-111","bipin","bgp",crs);
		System.out.println("student and course details from original object ");
		s1.getStudentDetails();
		System.out.println("original  student object ref  "+s1);
		System.out.println("original course object ref "+s1.crs);
		System.out.println();
		
		student s2=(student)s1.clone();
		System.out.println("student and course details from duplicate object ");
		s1.getStudentDetails();
		System.out.println("duplicate  student object ref "+s1);
		System.out.println("duplicate course object ref "+s1.crs);
		
		
		
	}
}

***************************

/* deep cloing */
/*user provide cloning */
class course{
	String cid,cname;
	int ccost;
	course(String cid,String cname,int ccost){
		this.cid=cid;
		this.cname=cname;
		this.ccost=ccost;
	}
}
class student implements Cloneable{
	String sid,sname,saddr;
	course crs;
	student(String sid,String sname,String saddr,course crs){
		this.sid=sid;
		this.sname=sname;
		this.saddr=saddr;
		this.crs=crs;
	}
	public void getStudentDetails(){
		System.out.println("student Details");
		System.out.println("student id :"+sid);
		System.out.println("student name :"+sname);
		System.out.println("student saddr :"+saddr);
		System.out.println("course Details");
		System.out.println("course id :"+crs.cid);
		System.out.println("course name :"+crs.cname);
		System.out.println("course cost :"+crs.ccost);
	}
	public Object clone() throws CloneNotSupportedException{
		course c=new course(crs.cid,crs.cname,crs.ccost);
		student s=new student(sid,sname,saddr,c);
		return s;
	}
	
}
class deppCloning {
	public static void main(String[] args)throws Exception{
		course crs=new course("c-111","java",1000);
		student s1=new student("s-111","bipin","bgp",crs);
		System.out.println("student and course details from original object ");
		s1.getStudentDetails();
		System.out.println("original  student object ref  "+s1);
		System.out.println("original course object ref "+s1.crs);
		System.out.println();
		
		student s2=(student)s1.clone();
		System.out.println("student and course details from duplicate object ");
		s1.getStudentDetails();
		System.out.println("duplicate  student object ref "+s1);
		System.out.println("duplicate course object ref "+s1.crs);
		
		
		
	}
}

***********************




***************************************************


ANNOTATION EXAMPLE

****************************************************
/* ANNOTATION   @override  */
class DBDriver{
	public void getDriver(){
	 System.out.println("Type-1 Driver");
	}
}
class DB_New_Driver extends DBDriver{
	@Override
	public void getdriver(){
	  System.out.println("Type-4 driver");
	}
}
class AnnotationOverride{
	public static void main(String []args){
	 DBDriver d=new DB_New_Driver();
	 d.getDriver();
	}
}	

/* compile time error 
give error
AnnotationOverride.java:8: error: method does not override or implement a method from a supertype
        @Override
		*/
*******************************************
/* AANOTATION @deprecated */
class Employee{
	@Deprecated
	public void gen_salary(long basic,float hq)//deprecated method
	{
	  float new_sal=basic+(basic*hq);
	  System.out.println("salary ="+new_sal);
	}
	public void gen_salary1(long basic,float hq, int ta,int bonus)//alternative method
	{
	   float new_sal=basic+(basic*hq)+ta+bonus;
	   System.out.println("salary ="+new_sal);
	}
}
class AnnotationDeprecated{
	public static void main(String []args){
	 Employee e=new Employee();
	 e.gen_salary(2500,0.15f);
	}
}

/* not compilation error after compiltion provide following message
Note: AnnotationDeprecated.java uses or overrides a deprecated API.

Note: Recompile with -Xlint:deprecation for details.
*/
***************************
/* ANNOTATION SuppressWarnings */
import java.util.*;
class customer{
	@SuppressWarnings("unchecked")
	public void list_customer(){
		ArrayList  al =new ArrayList();
		al.add("bipin");
		al.add("kumar");
		System.out.println(al);
	}
}
class AnnoSuppressWarnings{
	public static void main(String []args){
		customer c=new customer();
		c.list_customer();
	}
}
/*
without @SuppressWarnings(-----) compiler give following message
Note: AnnoSuppressWarnings.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
*/
******************************
		
/*custom Annotation part-1 */
import java.lang.annotation.*;
@Documented
@Inherited
@Target(ElementType.TYPE)
@Retention(RetentionPolicy.RUNTIME)
@interface Institute{
	String Name() default "B.C.E.BHAGALPUR";
	String Location() default "BHAGALPUR";
	String Contact_No() default "040-642515";
	String Website() default "www.bcebhagalpur.com";
}
------------

/* part -2 custome annotation*/
@Institute(Name="IIIT BHAGALPUR", Location="bgp",Contact_No="8083438299")
class Student{
	String sid,sname,saddr;
	Student(String sid,String sname,String saddr){
		this.sid=sid;
		this.sname=sname;
		this.saddr=saddr;
		
	}
	public void getStudentDetails(){
		System.out.println("Students Details ");
		System.out.println("=====================");
		System.out.println("Student id :"+sid);
		System.out.println("Student name :"+sname);
		System.out.println("Student address :"+saddr);
	}
}
------------

/* part -3 custom annotation  */
import java.lang.reflect.*;
class ClientApp{
	public static void main(String [] args){
	  Student std=new Student("1111","bipin","bgp");
	  std.getStudentDetails();
	  Class c =std.getClass();
	  Institute i=(Institute)c.getAnnotation(Institute.class);
	  System.out.println("institute Details ");
	  System.out.println("****************************");
	  System.out.println("name :"+i.Name());
	  System.out.println("Location :"+i.Location());
	  System.out.println("Contact_No :"+i.Contact_No());
	  System.out.println("Website :"+i.Website());
	}
}

***********************************

JAVA REFLECTION 


**********************************

/* java.lang.reflect.Field */
/* metadata of variables */
import java.lang.reflect.*;
class Employee11{
	public static final String eid="E-111";
	public static  String name="bipin";
	public static  float esal=5000.0f;
	
}
class Java_Lang_Field{
	public static void main(String []args)throws Exception{
	  Class c=Employee11.class;
	//  Field[] f=c.getDeclaredFields();
	  Field[] f=c.getFields();
	  for(Field f1:f){
		System.out.println("Field Name :"+f1.getName());
		System.out.println("Data Type :"+f1.getType().getName());
		
		int val=f1.getModifiers();
		System.out.println("Access Modifier :"+Modifier.toString(val));
		System.out.println("Field value :"+f1.get(f1));
		System.out.println();
		System.out.println("---------------------");
	  }
	}
}

*****************

/* java.lang.method */
/* metadata of method */
import java.lang.reflect.*;
import java.lang.*;
class Employee12{
	public static void create(String eid,String ename,float esal) throws
	java.sql.SQLException{}
	public final String search(String eid)throws 
	java.sql.SQLException{
	 return "";
	}
	public String update(String eid,String ename,float esal)throws java.rmi.RemoteException,java.sql.SQLException{
	return "";
	}
}
class Java_Lang_Method{
	public static void main(String []args)throws Exception{
	  Class c=Employee12.class;
	  Method[] method=c.getDeclaredMethods();
	  for(Method m:method){
	    System.out.println("Method name :"+m.getName());
		System.out.println("Return Type :"+m.getReturnType().getName());
		int val=m.getModifiers();
		System.out.println("Access modifier :"+Modifier.toString(val));
		Class[] cls1=m.getParameterTypes();
		System.out.println("Parameter Type");
		for(Class c1:cls1){
		  System.out.println(c1.getName()+" ");
		}
		System.out.println();
		Class[] cls2=m.getExceptionTypes();
		System.out.println("Exception Type ");
		for(Class c2:cls2){
		 System.out.println(c2.getName()+" ");
		 
		}
		System.out.println();
	  }
	}
}

***********************

/* java.lang.Constructor */
/* metadate of constructor */
import java.lang.reflect.*;
class Employee13{
	public Employee13(String eid,String ename,float esal)throws java.sql.SQLException{
	}
	public Employee13(String eid,String ename)throws java.rmi.RemoteException,java.sql.SQLException{
	}
	
}
class Java_Lang_Constructor{
	public static void main(String []args){
		Class cls=Employee13.class;
		Constructor[] cons=cls.getDeclaredConstructors();
		for(Constructor c:cons){
		  System.out.println("Constructor Name :"+c.getName());
		  int val=c.getModifiers();
		  System.out.println("Access modifier :"+Modifier.toString(val));
		  Class[] cls1=c.getParameterTypes();
		  System.out.println("Parameter Type");
		  for(Class c1:cls1){
		   System.out.println(c1.getName());
		  }
		  System.out.println();
		  
		  Class[] cls2=c.getExceptionTypes();
		  System.out.println("Exception type ");
		  for(Class c2:cls2){
		  System.out.println(c2.getName());
		  }
		  System.out.println();
		  
		  System.out.println("========================");
		  
		}
	}
}

**************************

/* reflection API */
/* metadata of class */
import java.lang.reflect.*;
abstract class Employee10 implements Serializable{
	{	
}
class Java_Lang_Class {
	public static void main(String []args){
		Class c =Class.forName("Employee10");
		System.out.println("Name :"+c.getName());
		System.out.println("superClass :"+c.getSuperclass().getName());
		Class cls[]=c.getInterfaces();
		System.out.println("Interface :");
		for(Class cl:cls){
			System.out.println(cl.getName());
		}
		System.out.println();
		int i=c.getModifiers();
		System.out.println("modifier :"+Modifier.toString(i));
	}
} 

this programing is not run   
**********************************************************

NETWORKING IN JAVA 



***********************************************************

/* inner class in java */
class Outer{
	int i=10;
	void m1(){
		System.out.println("outer m1() method ");
		//System.out.println(j); error
	}
	class Inner{
		//static int k1=30;  error
		static final int k=30;
		int j=20;
		void m2(){
			System.out.println("inner m2() method ");
			System.out.println(i);
		}
		void m3(){
			System.out.println("inner m3() method ");
		}
	}
}
class Outer_Inner{
	public static void main(String []args){
		Outer o=new Outer();
		o.m1();
		//o.m2(); error
		Outer.Inner oi=new Outer().new Inner();
		oi.m2();
		//oi.m1(); error
		oi.m3();
		
	}
}

*************************

/* inner class inherited to another inner class within same outer class */
class Outer1{
     class Inner1{
	   void m1(){
		System.out.println("Inner1 m1() method ");
		
	   }
	 }
	 class Inner2 extends Inner1{
	   void m2(){
	     System.out.println(" Inner2 m2() method ");
	   }
    }
}
class Inner_Inherited{
	public static void main(String []args){
	  Outer1.Inner1 oi1=new Outer1().new Inner1();
	  oi1.m1();
	  Outer1.Inner2 oi2=new Outer1().new Inner2();
	  oi2.m1();
	  oi2.m2();
	}
}

*********************

/* override outer class method to iner class method */
class A {
    void m1(){
        System.out.println("m1-A");
    }
    class B extends A{
        void m1(){
            System.out.println("m1-B");
        }
    }
    
}
class Inner_Override{
    public static void main(String []args){
        A a=new A().new B();
        a.m1();
    }
}

*******************

/* interface in inner class */
class Outer3{
	interface I{
	  void m1();
	  void m2();
	  
	}
	class Inner4 implements I{
		public void m1(){
		  System.out.println("m1()-B");
		}
		public void m2(){
		  System.out.println("M2()-B");
		}
	}
}
class InterfaceInInnerClass{
	public static void main(String []args){
	  Outer3.I oi =new Outer3().new Inner4();
	  oi.m1();
	  oi.m2();
	}
}

**********************

/*NETWORKING IN JAVA */
/* abstract class in inner class */
class Outer5{
	abstract class Inner5{
		void m1(){
			System.out.println("m1-Inner5");
			
		}
		abstract void m2();
		abstract void m3();
	}
	class Inner6 extends Inner5{
		void m2(){
		System.out.println("m2-Inner6");
		}
		void m3(){
		  System.out.println("m3-Inner6");
		}
	}
}
class AbstractInInner{
	public static void main(String []args){
	  Outer5.Inner5 oi1=new Outer5().new Inner6();
	  oi1.m1();
	  oi1.m2();
	  oi1.m3();
	  
	}
}

*********************

/* networking in java */
/* static inner class */
class Outer7{
	int i=10;
	static int j=20;
	void m1(){
	  System.out.println("m1-outer7");
	}
	
	static class Inner7{
	   static int k=30;
	   void m2(){
			System.out.println("m2-Inner7");
			//System.out.println(i);  error
			System.out.println(j);
	   }
	   static void m3(){
	     System.out.println("m3-Inner7");
	   }
	}
	
}
class StaticInInner{
	public static void main(String []args){
	  Outer7 o=new Outer7();
	  o.m1();
	  Outer7.Inner7 oi=new Outer7.Inner7();
	  oi.m2();
	  oi.m3();
	  Outer7.Inner7.m3();
	}
}

**************************

/* class inside interface */
interface I{
	class A{
	  void m1(){
	    System.out.println("m1-A");
	  }
	  void m2(){
	    System.out.println("m2-A");
	  }
	}
}
class ClassInInterface{
	public static void main(String []args){
	    I.A ia=new I.A();
		ia.m1();
		ia.m2();
	}
 }
 
**********************

/*classes ,abstract classes and interface in interface */
interface I1{
		abstract class A{
			void m1(){
					System.out.println("m1-abstract A");
			}
			abstract void m2();
			abstract void m3();
			
		}
		class B extends A{
		   void m2(){
				System.out.println("m2-B");
		   }
		   void m3(){
				System.out.println("m3-B");
		   }
		}
}
class InsideInterface{
	public static void main(String []args){
		I1.A ia=new I1.B();
		ia.m1();
		ia.m2();
		ia.m3();
	}
}
*************************** 



/* METHOD LOCAL INNER CLASS */
/* DECLARING A CLASS INSIDE A METHOD */
class A{
	void method(){
		class B{
			void m1(){
				System.out.println("m1-B");
			}
			void m2(){
				System.out.println("m2-B");
			}
		}
		B b=new B();
		b.m1();
		b.m2();
	}
}
class ClassInMethod{
	public static void main(String []args){
		A a=new A();
		a.method();
		
	}
}
*****************************

/* ANONYMOUS INNER CLASS */
/* with interface */
interface I{
	void m1();
	void m2();
	
}
class A{
 I i=new I()
 {
		public void m1(){
			System.out.println("m1-AC");
		}
		public void m2(){
			System.out.println("m2-AC");
		}
		public void m3(){
			System.out.println("m3-AC");
		}
 };
}
class AnonymousInnerClass{
	public static void main(String []args){
		A a=new A();
		a.i.m1();
		a.i.m2();
		//a.i.m3();  error
	}
}

**************************

/* anonymous class for abstract class */
abstract class A{
	void m1(){
		System.out.println("m1-A");
	}
	abstract void m2();
	abstract void m3();
}
class B{
	A a=new A()
	{
		void m2(){
			System.out.println("m2-AC");
		}
		void m3(){
			System.out.println("m3-AC");
		}
	};
}
class anonymousAbstractClass{
	public static void main(String []args){
		B b=new B();
		b.a.m1();
		b.a.m2();
		b.a.m3();
	}
}

**************************************

INTERNATIONALIZATION  


**************************************

/* internationalization */
/* use to locale convertion */
/*
import java.util.*;
import java.text.*;
public class NumberFormatI18N{
	public static void main(String []args)throws Exception{
		Locale l=new Locale( "en","IN");
		NumberFormat nf=new NumberFormat.getInstance(l);
		System.out.println(nf.format(12345.2345));
	}
}
  not run 
*/

import java.text.NumberFormat;  
import java.util.*;  
  
public class NumberFormatI18N {  
  
static void printNumber(Locale locale){  
 double dbl=105000.3245;  
 NumberFormat formatter=NumberFormat.getNumberInstance(locale);  
 String number=formatter.format(dbl);  
 System.out.println(number+" for the locale "+locale);  
}  
  
public static void main(String[] args) {  
    printNumber(Locale.UK);  
    printNumber(Locale.US);  
    printNumber(Locale.FRANCE);  
    printNumber(Locale.JAPAN);  
  
}  
}  


  CURRENCY FORMAT  
  
  import java.text.NumberFormat;  
import java.util.*;  
public class CurrencyFormatI18N {  
  
static void printCurrency(Locale locale){  
 double dbl=10500.3245;  
 NumberFormat formatter=NumberFormat.getCurrencyInstance(locale);  
 String currency=formatter.format(dbl);  
 System.out.println(currency+" for the locale "+locale);  
}  
  
public static void main(String[] args) {  
    printCurrency(Locale.UK);  
    printCurrency(Locale.US);  
    printCurrency(Locale.FRANCE);  
}  
}  


***********************

/* date formation  internationalization */
/*
import java.util.*;
import java.text.*;
class DateFormatI18N{
public static void main(String []args) throws Exception{
	Locale l=new Locale("en","US");
	DateFormat df=new DateFormat.getDateInstance(0,l);
	String s=df.format(new Date());
	System.out.println(s);
}
} not run 
*/


import java.text.DateFormat;  
import java.util.*;  
public class DateFormatI18N{  
      
static void printDate(Locale locale){ 
 
DateFormat formatter=DateFormat.getDateInstance(DateFormat.DEFAULT,locale);  
Date currentDate=new Date();  
String date=formatter.format(currentDate);  
System.out.println(date+" "+locale);  
}  
  
public static void main(String[] args) {  
    printDate(Locale.UK);  
    printDate(Locale.US);  
    printDate(Locale.FRANCE);  
}  
}  


/* 
  //TIME FORMAT ***
import java.text.DateFormat;  
import java.util.*;  
  
public class InternationalizingTime {  
  
static void printTime(Locale locale){  
DateFormat formatter=DateFormat.getTimeInstance(DateFormat.DEFAULT,locale);  
Date currentDate=new Date();  
String time=formatter.format(currentDate);  
System.out.println(time+" in locale "+locale);  
}  
  
public static void main(String[] args) {  
printTime(Locale.UK);  
printTime(Locale.US);  
printTime(Locale.FRANCE);  
}  
}  */


************************


/* internationalization message format */
/*
import java.util.*;
import java.text.*;

public class MessageFormatI18N{
	public static void main(String []args)throws Exception{
			Locale l=new Locale("en","US");
			ResourceBundle rb=new ResourceBundle.getBundle("abc",l);
			System.out.println(rb.getString("Welcome"));
	}
} not run
*/

import java.util.Locale;  
import java.util.ResourceBundle;  
public class MessageFormatI18N {  
 public static void main(String[] args) {  
  
  ResourceBundle bundle = ResourceBundle.getBundle("MessageBundle", Locale.US);  
  System.out.println("Message in "+Locale.US +":"+bundle.getString("greeting"));  
  
  //changing the default locale to indonasian   
  Locale.setDefault(new Locale("in", "ID"));  
  bundle = ResourceBundle.getBundle("MessageBundle");  
  System.out.println("Message in "+Locale.getDefault()+":"+bundle.getString("greeting"));  
  
 }  
}  

********************************************************

IOSTREAM 


********************************************************

/*IOSTREAM*/
/* FILE OPERATION :-FileOutputStream */
import java.io.*;
public class FileOutputStreamEx{
	public static void main(String []args)throws Exception{
		FileOutputStream fos=new FileOutputStream("fileoutputstream.txt");//1.FileOutputStream object create
		String data="Bhagalpur Colege Of Engineering";//2.declare data which is transfer 
		byte[] b=data.getBytes();//3.convert data from string to byte
		fos.write(b);//4. write byte[] data to FileOutputStream
		fos.close();//5.closing FileOutputStream
	}
}

**********************

/* IOSTREAM */
/* FileInputStream */
import java.io.*;
public class FileInputStreamEx{
		public static void main(String []args)throws Exception{
				FileInputStream fis=new FileInputStream("fileinputstream.txt");//create FileImageInputStream object
				int size=fis.available();//get data size available in FileImageInputStream
				byte[] b=new byte[size];//
				fis.read(b);//read data from FileImageInputStream
				String str=new String(b);
				System.out.println(str);
				fis.close();
		}
}
***************************

/* IOSTREAM */
/* FileReader */
import java.io.*;
public class FileReaderEx{
		public static void main(String []args)throws Exception{
			FileReader fr=new FileReader("filereader.txt");//create object
			String data="";
			int val=fr.read();//read ascii value  from filereader
			while(val!=-1){
				data=data+(char)val;//convert ascii value into character and append all  
				val=fr.read();//
			}
			System.out.println(data);
			fr.close();
		}
}

*********************
/* IOSTREAM */
/*FileWriter */
import java.io.*;
public class FileWriterEx{
	public static void main(String []args)throws Exception{
		FileWriter fw=new FileWriter("filewriter.txt",true);
		String data="Bhagalpur Collee Of Engineering ";
		char[] ch=data.toCharArray();
		fw.write(ch);
		fw.close();
	}
}

*********************

/* write a prgm to take data from a text file and to display the no of words available in the text file */
import java.io.*;
import java.util.*;
public class FileInputAndOutput{
	public static void main(String []args)throws Exception{
		FileInputStream fis=new FileInputStream("fileinputstream.txt");
		int size=fis.available();
		byte[] b=new byte[size];
		fis.read(b);
		String data=new String(b);
		StringTokenizer st=new StringTokenizer(data);
		int count=st.countTokens();
		System.out.println("No. of word :"+count);
		int isCount=0;
		while(st.hasMoreTokens()){
				String token=st.nextToken();
				if(token.equals("is")){
				  isCount=isCount+1;
				  
				}
		}
		System.out.println("15 is repeated :"+isCount);
		
	}
}
************************

/* write a java prgm to display a file context on command prompt by taking filename as command line argument */
import java.io.*;
public class InputFromCommandP{
   public static void main(String[] args)throws Exception{
		String fname=args[0];
		FileReader fr=new FileReader(fname);
		String data="";
		int val=fr.read();
		while(val!=-1){
		  data=data+(char)val;
		  val=fr.read();
		}
		System.out.println(data);
		fr.close();
   }
} 
**************************

/* dynamic input from BufferedReader  */
import java.io.*;
public class BufferedReaderEx{
	public static void main(String[] args)throws Exception{
		BufferedReader br=new BufferedReader(new InputStreamReader(System.in));
		System.out.print("Enter a text :");
		String data1=br.readLine();
		System.out.print("Enter the same text again");
		int data2=br.read();
		System.out.println("First Entered :"+data1);
		System.out.println("Second Enterd :"+data2);
		}
}

************************


import java.io.*;

public class BufferedReaderEx1{
	public static void main(String[] args)throws Exception{
		BufferedReader br=new BufferedReader(new InputStreamReader(System.in));
		System.out.print("first value :");
		String fval=br.readLine();
		System.out.print("Second value :");
		String sval=br.readLine();
		System.out.println("Addition :"+fval+sval);
		int val1=Integer.parseInt(fval);
		int val2=Integer.parseInt(sval);
		System.out.println("Addition :"+(val1+val2));
	}
}
****************

/* Scanner in IOStream */
import java.io.*;
import java.util.*;
public class ScannerEx{
		public static void main(String []args)throws Exception{
			Scanner s=new Scanner(System.in);
			System.out.print("Employee id :");
			String eid=s.next();
			System.out.print("Employee Name :");
			String ename=s.nextLine();
			System.out.print("Employee Address :");
			String eadd=s.nextLine();
			System.out.print("Employee Age :");
			int eage=s.nextInt();
			System.out.print("Employee Salary :");
			float esal=s.nextFloat();
			System.out.println("Employee Details ");
			System.out.println("-------------------");
			System.out.println("Employee Name :"+ename);
			System.out.println("Employee Id :"+eid);
			System.out.println("Employee Address :"+eadd);
			System.out.println("Employee Age :"+eage);
			System.out.println("Employee Salary :"+esal);
			
		}
}

*********************

/* Console in IOSTREAM */
import java.io.*;
public class ConsoleEx{
		public static void main(String []args)throws Exception{
			Console c=System.console();
			String uname=c.readLine("user Name :");
			char[] pwd=c.readPassword("password :");
			String upwd=new String(pwd);
			if(uname.equals("bipin")&&upwd.equals("bipin")){
				System.out.println("status :valid user");
				
			}
			else{
				System.out.println("status : Invalid user ");
			}
		}
}


****************************************************************************************************************************
****************************************************************************************************************************
****************************************************************************************************************************
****************************************************************************************************************************

		JDBC     in Eclips      set build path in each program 
		
*****************************************************************************************************************************
*****************************************************************************************************************************
*****************************************		*****************************************************************************
		
/* WORKING WITH TYPE -2 DRIVER */
/* type 2 driver */
package jdbcApp1;
import java.sql.*;        
public class jdbcApp1 {

	public static void main(String[] args)throws Exception {
				//load and register driver class (optional)
				Class.forName("oracle.jdbc.OracleDriver");
				//Established connection b/w java app and database
				Connection con=DriverManager.getConnection("jdbc:oracle:oci:@ORCL","system","oracle");
				//create statement 
				Statement st=con.createStatement();
				//execute query 
				ResultSet rs=st.executeQuery("select *from dept");
				while(rs.next()){
					System.out.println(rs.getInt(1)+" "+rs.getString(2)+" "+rs.getString(3));
					
				} 
				con.close();

	}

}


*****************************

/* WORKING WITH TYPE -4 DRIVER */
/* type 4 driver */
package jdbcApp2;
import java.sql.*;
public class jdbcApp2 {

	public static void main(String[] args)throws Exception {
		//load and register driver class (optional)
		Class.forName("oracle.jdbc.OracleDriver");
		//Established connection b/w java app and database
		Connection con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:ORCL","system","oracle");
		//create statement 
		Statement st=con.createStatement();
		//execute query 
		ResultSet rs=st.executeQuery("select *from dept");
		while(rs.next()){
			System.out.println(rs.getInt(1)+" "+rs.getString(2)+" "+rs.getString(3));
			
		} 
		con.close();
	}

}


*******************************

/*  the following example demonstrate how to create a table on database through a jdbc appliction 
 by taking table name as dynamic 
 */
package jdbcApp01;
import java.sql.*;
import java.io.*;
public class jdbcApp01 {

	public static void main(String[] args)throws Exception {
		//load a register driver
		Class.forName("oracle.jdbc.OracleDriver");
		//established connection b/w java appl and database
		Connection con =DriverManager.getConnection
				("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
		//prepare statement
		Statement st=con.createStatement();
		//create BufferedReader
		BufferedReader br=new BufferedReader(new InputStreamReader(System.in));
		//take table name as dynamic input
		System.out.println("Enter table Name");
		String tname=br.readLine();
		//prepare sqlquery
		String sql="create table "+tname+"(eno number,ename varchar2(10),esal number)";
		//execute sqlquery
		st.executeUpdate(sql);
		System.out.println("table created successfuly");
		//close conection
		con.close();
		
		

	}

}
******************************
/* the following example demonstrate how to insert no of records on database 
 * table by taking record data as dynamically */ 
 
package jdbcApp02;
import java.sql.*;
import java.io.*;
public class jdbcApp2 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection
				("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
		Statement st=con.createStatement();
		BufferedReader br=new BufferedReader(new InputStreamReader(System.in));
		while(true){
			System.out.println("Employee Number :");
			int eno=Integer.parseInt(br.readLine());
			System.out.println("Employee Name :");
			String ename=br.readLine();
			System.out.println("Employee Salary :");
			float esal=Float.parseFloat(br.readLine());
			st.executeUpdate("insert into emp1 values ("+eno+",'"+ename+"','"+esal+"')");
			System.out.println("Employee Inserted successfully");
			System.out.println("One more Employee[yes/no]? :");
			String option=br.readLine();
			if(option.equals("no")){
				break;
			}
			
			
			
		}
		con.close();
	}

}
********************************

/* the following example demonstrate how to perform updations on
 *  database table through jdbc application
 */
package jdbcApp03;
import java.sql.*;
import java.io.*;

public class jdbcApp03 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection
				("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
		Statement st=con.createStatement();
		BufferedReader br=new BufferedReader(new InputStreamReader(System.in));
		System.out.println("Bonus Amount :");
		int bonus_amt=Integer.parseInt(br.readLine());
		System.out.println("Salary range :");
		float sal_range=Float.parseFloat(br.readLine());
		int rowCount=st.executeUpdate("update emp1 set esal=esal+"+bonus_amt+" where esal<"+sal_range);
		System.out.println("Employee Updated :"+rowCount);
				con.close();
		
	}

}
*******************************
/* the foolowing example demonstrate how to delete no of records from database 
 * table through a jdbc application
 */
package jdbcApp04;
import java.sql.*;
import java.io.*;
public class jdbcApp04 {

	public static void main(String[] args)throws Exception {
		//DriverManager.registerDriver(new oracle.jdbc.OracleDriver());
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection
				("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
		Statement st=con.createStatement();
		BufferedReader br=new BufferedReader(new InputStreamReader(System.in));
		System.out.println("Salary Range :");
		float sal_range=Float.parseFloat(br.readLine());
		int rowCount=st.executeUpdate("delete from emp1 where esal<"+sal_range);
		System.out.println("Record Deleted :"+rowCount);
		con.close();

	}

}
***************************

/* the following example demonstrate how to fetch the data from database through Resultset object
 
 */
package jdbcApp05;
import java.sql.*;

public class jdbcApp05 {

	public static void main(String[] args) throws Exception{
		 //OracleDriver driver=new OracleDriver();
		Class.forName("oracle.jdbc.OracleDriver"); 
		Connection con =DriverManager.getConnection
				 ("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
		 Statement st=con.createStatement();
		 ResultSet rs=st.executeQuery("select *from emp1");
		 System.out.println("ENO\tENAME\tESAL");
		 System.out.println("------------------");
		 while(rs.next()){
			 System.out.println(rs.getInt(1)+"\t"+rs.getString(2)+"\t"+rs.getString(3));
		 }
		 		
		con.close();
	}

}
******************************

/* using ResultSet in selected query */
package jdbcApp06;
import java.sql.*;
public class jdbcApp06 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection
				("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
		Statement st=con.createStatement();
		boolean b=st.execute("select *from emp1");
		System.out.println(b);
		ResultSet rs=st.getResultSet();
		System.out.println("ENO\tENAME\tESAL");
		System.out.println("------------------");
		while(rs.next()){
			System.out.println(rs.getInt(1)+"\t"+rs.getString(2)+"\t"+rs.getString(3));
			
		}
		con.close();
	}

}
*******************************
/* execute() method when updation group sql query used */
package jdbcApp07;
import java.sql.*;
public class jdbcApp07 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con =DriverManager.getConnection
				("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
		Statement st=con.createStatement();
		boolean b=st.execute("update emp1 set esal=esal+100");
		System.out.println(b);
		int rowCount=st.getUpdateCount();
		System.out.println("Record Updated :"+rowCount);
		con.close();

	}

}
*******************************

/* updation query use in executeQuery()*/
package jdbcApp08;
import java.sql.*;
public class jdbcApp08 {

	public static void main(String[] args) {
		Statement st=null;
		try{
			Class.forName("oracle.jdbc.OracleDriver");
			Connection con=DriverManager.getConnection
					("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
			st=con.createStatement();
			ResultSet rs=st.executeQuery("update emp1 set sal=sal+100");
			int rowCount=st.getUpdateCount();
			System.out.println("Record Updated :"+rowCount);
			
		}
		catch(Exception e){
			e.printStackTrace();
		}
	}

}

this give an exception
**************************************

/* selected query use in executeUpdate() */
package jdbcApp09;
import java.sql.*;
public class jdbcApp09 {

	public static void main(String[] args) {
		try{
			Class.forName("oracle.jdbc.OracleDriver");
			Connection con=DriverManager.getConnection
					("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
			Statement st=con.createStatement();
			int rowCount=st.executeUpdate("select *from emp1");
			System.out.println("Row Count :"+rowCount);
			ResultSet rs=st.getResultSet();
			System.out.println("ENO\tENAME\tESAL");
			System.out.println("-------------------");
			while(rs.next()){
				System.out.println(rs.getInt(1)+"\t"+rs.getString(2)+"\t"+rs.getShort(3));
				
			}
					
		}catch(Exception e){
			e.printStackTrace();
		}
	}

}
*******************************

/* the following example demonstrate how to retrieve the data from database and 
 * how to display that data through an HTML page
 */
package jdbcApp10;
import java.io.FileOutputStream;
import java.sql.*;
public class jdbcApp10 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection
				("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
		Statement st=con.createStatement();
		ResultSet rs=st.executeQuery("select *from emp1");
		String data="";
		data=data+"<html><body><center><table border='1' bgcolor='lightblue'>";
		data=data+"<tr><td>ENO</td><td>ENAME</td><td>ESAL</td></tr>";
		while(rs.next()){
			data=data+"<tr>";
			data=data+"<td>"+rs.getInt(1)+"</td><td>"+rs.getString(2)+"</td><td>"+rs.getString(3)+"</td>";
			data=data+"</tr>";
		}
		data=data+"</table></center></body></html>";
		FileOutputStream fos=new FileOutputStream("emp.html",true);
		byte[] b=data.getBytes();
		fos.write(b);
		System.out.println("Open emp.html file to get Employee data");
		fos.close();
		con.close();
	}

}
**************************************************************
**************************************************************
LoginFrame.java

package jdbcApp11;
import java.awt.Button;
import java.awt.Color;
import java.awt.FlowLayout;
import java.awt.Font;
import java.awt.Frame;
import java.awt.Graphics;
import java.awt.GraphicsConfiguration;
import java.awt.HeadlessException;
import java.awt.Label;
import java.awt.TextField;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.awt.event.WindowAdapter;
import java.awt.event.WindowEvent;
public class LoginFrame extends Frame implements ActionListener{
	Label l1,l2;
	TextField tf1,tf2;
	Button b1;
	String status="";
	public LoginFrame(){
		this.setVisible(true);
		this.setSize(500, 500);
		this.setTitle("Login Frame");
		this.setBackground(Color.pink);
		this.setLayout(new FlowLayout());
		this.addWindowListener(new WindowAdapter(){
			public void windowClosing(WindowEvent we){
				System.exit(0);
			}
		});
		
		l1=new Label("User Name ");
		l2=new Label("Password ");
		tf1=new TextField(20);
		tf2=new TextField(20);
		tf2.setEchoChar('*');
		b1=new Button("Login");
		b1.addActionListener(this);
		Font f=new Font("arial",Font.BOLD,20);
		l1.setFont(f);
		l2.setFont(f);
		tf1.setFont(f);
		tf2.setFont(f);
		b1.setFont(f);
		this.add(l1);
		this.add(l2);
		this.add(tf1);
		this.add(tf2);
		this.add(b1);
		
	}
	public void actionPerformed(ActionEvent ae){
		String uname=tf1.getText();
		String upwd=tf2.getText();
		UserService us=new UserService();
		status=us.checkLogin(uname,upwd);
		repaint();
	}
	public void paint(Graphics g){
		Font f=new Font("arial",Font.BOLD,30);
		g.setFont(f);
		g.drawString("Staus :"+status, 50, 250);
	}
}



UserService.java

package jdbcApp11;
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.ResultSet;
import java.sql.Statement;

public class UserService {
	Connection con;
	Statement st;
	ResultSet rs;
	String status="";
	public UserService(){
		try{
			Class.forName("oracle.jdbc.OracleDriver");
			con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
			st=con.createStatement();
		}catch(Exception e){
			e.printStackTrace();
		}
	}
public String checkLogin(String uname,String upwd){
	try{
		rs=st.executeQuery("select *from  register_users where uname='"+uname+"'and upwd='"+upwd+"'");
		boolean b=rs.next();
		if(b==true){
			status="Login Success";
			
		}else{
			status="Login Failure";
		}
	}catch(Exception e){
		e.printStackTrace();
	}
	return status;
}
	
}


jdbcApp11.java

package jdbcApp11;
public class jdbcApp11 {

	public static void main(String[] args) {
		LoginFrame lf=new LoginFrame();
	}

}
*************************************************************
*************************************************************

EmployeeAddFrame.java

package jdbcApp12;
import java.awt.*;
import java.awt.event.*;
public class EmployeeAddFrame extends Frame implements ActionListener {
Label l1,l2,l3,l4;
TextField tf1,tf2,tf3,tf4;
Button b1;
String status="";
public EmployeeAddFrame(){
	this.setVisible(true);
	this.setSize(500, 500);
	this.setTitle("Employee Registration Frame");
	this.setBackground(Color.cyan);
	this.setLayout(null);
	this.addWindowListener(new WindowAdapter(){
		public void windowClosing(WindowEvent we){
			System.exit(0);
		}
	});
	l1=new Label("Employee Number");
	l2=new Label("Employee Name");
	l3=new Label("Emolyee Salary");
	l4=new Label("Employee Address");
	tf1=new TextField(20);
	tf2=new TextField(20);
	tf3=new TextField(20);
	tf4=new TextField(20);
	b1=new Button("ADD");
	b1.addActionListener(this);
	Font f=new Font("arial",Font.BOLD,20);
	l1.setFont(f);
	l2.setFont(f);
	l3.setFont(f);
	l4.setFont(f);
	tf1.setFont(f);
	tf2.setFont(f);
	tf3.setFont(f);
	tf4.setFont(f);
	b1.setFont(f);
	l1.setBounds(50,100,200,25);
	tf1.setBounds(250,100,200,30);
	l2.setBounds(50,150,200,25);
	tf2.setBounds(250,150,200,30);
	l3.setBounds(50,200,200,25);
	tf3.setBounds(250,200,200,30);
	l4.setBounds(50,250,200,25);
	tf4.setBounds(250,250,200,30);
	b1.setBounds(50,300,100,30);
	this.add(l1);
	this.add(tf1);
	this.add(l2);
	this.add(tf2);
	this.add(l3);
	this.add(tf3);
	this.add(l4);
	this.add(tf4);
	this.add(b1);
		
}
public void actionPerformed(ActionEvent ae){
	try{
		int eno=Integer.parseInt(tf1.getText());
		String ename=tf2.getText();
		float esal=Float.parseFloat(tf3.getText());
		String eaddr=tf4.getText();
		EmployeeService es=new EmployeeService();
		status=es.add(eno,ename,esal,eaddr);
		repaint();
	}catch(Exception e){
		e.printStackTrace();
	}
}
public void paint(Graphics g){
	Font f=new Font("arial",Font.BOLD,30);
	g.setFont(f);
	g.drawString("Status:"+status, 50, 400);
}

}


EmployeeService.java


package jdbcApp12;
import java.sql.*;
public class EmployeeService {
Connection con;
Statement st;
ResultSet rs;
String status="";
public EmployeeService(){
	try{
		Class.forName("oracle.jdbc.OracleDriver");
		con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
		st=con.createStatement();
		
	}catch(Exception e){
		e.printStackTrace();
	}
}
public String add(int eno,String ename,float esal,String eaddr){
	try{
		rs=st.executeQuery("select *from emp1 where eno="+eno);
		boolean b=rs.next();
		if(b==true){
			status="Employee Existed Already";
		}else{
			st.executeUpdate("insert into emp1 values("+eno+",'"+ename+"',"+esal+",'"+eaddr+"')");
			status="Employee Registration Success";
			
		}
	}catch(Exception e){
		status="Employee Registration Failure";
		e.printStackTrace();
	}
	return status;
}
}


jdbcApp12.java

package jdbcApp12;

public class jdbcApp12 {

	public static void main(String[] args) {
		EmployeeAddFrame f=new EmployeeAddFrame();
	}

}
****************************************************************
****************************************************************


StudentSearchFrame.java

package jdbcApp13;
import java.awt.*;
import java.awt.event.*;
public  class StudentSearchFrame extends Frame implements ActionListener{
	Label l1;
	TextField tf1;
	Button b1;
	StudentTo sto;
	public StudentSearchFrame(){
		this.setVisible(true);
		this.setSize(500,500);
		this.setTitle("Student Search Frame");
		this.setLayout(new FlowLayout());
		this.setBackground(Color.green);
		this.addWindowListener(new WindowAdapter(){
			public void windowClosing(WindowEvent we){
				System.exit(0);
			}
		});
		l1=new Label("Student Id");
		tf1=new TextField(20);
		b1=new Button("Search");
		b1.addActionListener(this);
		
		Font f=new Font("arial",Font.BOLD,20);
		l1.setFont(f);
		tf1.setFont(f);
		b1.setFont(f);
		this.add(l1);
		this.add(tf1);
		this.add(b1);
	}
	
	public void actionPerformed(ActionEvent ae){
		String sid=tf1.getText();
		StudentService ss=new StudentService();
		sto=ss.search(sid);
		repaint();
		
	}
	public void paint(Graphics g){
		Font f=new Font("arial",Font.BOLD,30);
		g.setFont(f);
		if(sto==null){
			g.drawString("Student Not Existed", 50, 300);
			
		}else{
			g.drawString("Student Id :"+sto.getSid(), 50, 250);
			g.drawString("Student Name :"+sto.getSname(), 50, 300);
			g.drawString("Student Address:"+sto.getSaddr(), 50, 350);
		}
	}
	
}



StudentService.java

package jdbcApp13;
import java.sql.*;
public class StudentService {
	Connection con;
	Statement st;
	ResultSet rs;
	StudentTo sto;
	public StudentService(){
		try{
			Class.forName("oracle.jdbc.OracleDriver");
			con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
			st=con.createStatement();
		}catch(Exception e){
			//e.printStackTrace();
		}
	}
	public StudentTo search(String sid){
		
		try{
			rs=st.executeQuery("select *from student where sid="+sid);
			boolean b=rs.next();
			if(b==true){
				sto=new StudentTo();
				sto.setSid(rs.getString(1));
				sto.setSname(rs.getString(2));
				sto.setSaddr(rs.getString(3));
			}else{
				sto=null;
			}
		}catch(Exception e){
			e.printStackTrace();
		}
		return sto;
	}
	
}


StudentTo.java

package jdbcApp13;

public class StudentTo {
	private String sid;
	private String sname;
	private String saddr;
	public String getSid(){
		return sid;
	}
	public void setSid(String sid){
		this.sid=sid;
		
	}
	public String getSname(){
		return sname;
	}
	public void setSname(String sname){
		this.sname=sname;
	}
	public String getSaddr(){
		return saddr;
	}
	public void setSaddr(String saddr){
		this.saddr=saddr;
	}
		

}



jdbcApp13.java

package jdbcApp13;

public class jdbcApp13 {

	public static void main(String[] args) {
		StudentSearchFrame sf=new StudentSearchFrame();
	}

}


*********************************************************
*********************************************************
/* the example illustrate the forward and backward direction of ResultSet
 * 
 */
package jdbcApp15;
import java.sql.*;
public class jdbcApp15 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection(
				"jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
	    Statement st=con.createStatement(ResultSet.TYPE_SCROLL_SENSITIVE,ResultSet.CONCUR_UPDATABLE);
	    ResultSet rs=st.executeQuery("select *from emp1");
	    System.out.println("Data in Forward Direction ");
	    System.out.println("ENO\tENAME\tESAL\tEADDR\t");
	    System.out.println("-----------------------------");
	    while(rs.next()){
	    	System.out.println(rs.getInt(1)+"\t"+rs.getString(2)+"\t"+rs.getFloat(3)+"\t"+rs.getString(4));
	    	
	    }
	    System.out.println();
	    System.out.println("Data in Backward Direction");
	    System.out.println("ENO\tENAME\tESAL\tEADDR\t");
	    System.out.println("----------------------------");
	    while(rs.previous()){
	    	System.out.println(rs.getInt(1)+"\t"+rs.getString(2)+"\t"+rs.getFloat(3)+"\t"+rs.getString(4));
	    }
	    con.close();
	}

}

****************************************************
***************************************************
/* the example illustrate the scroll type ResultSet and Updatable ResultSet 
 * 
 */
package jdbcApp16;
import java.sql.*;
public class jdbcApp16 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
		Statement st=con.createStatement(ResultSet.TYPE_SCROLL_SENSITIVE,ResultSet.CONCUR_UPDATABLE);
		ResultSet rs=st.executeQuery("select *from emp1");
		rs.afterLast();
		rs.previous();
		System.out.println(rs.getInt(1));
		System.out.println();
		rs.beforeFirst();
		rs.next();
		System.out.println(rs.getInt(1));
		System.out.println();
		rs.last();
		System.out.println(rs.getInt(1));
		System.out.println();
		rs.first();
		System.out.println(rs.getInt(1));
		System.out.println();
		rs.absolute(3);
		System.out.println(rs.getInt(1));
		System.out.println();
		rs.absolute(-3);
		System.out.println(rs.getInt(1));
		System.out.println();
		rs.first();
		rs.relative(2);
		System.out.println(rs.getInt(1));
		System.out.println();
		rs.last();
		rs.relative(-2);
		System.out.println(rs.getInt(1));
		System.out.println();
	}

}
****************************************************
****************************************************


jdbcApp17.java

package jdbcApp17;
import java.awt.*;
import java.awt.event.*;
public class PlayerFrame extends Frame implements ActionListener{
	Button b1,b2,b3,b4;
	String label;
	EmployeeTo eto;
	EmployeeService es;
	public PlayerFrame(){
		this.setVisible(true);
		this.setSize(500, 500);
		this.setTitle("Player Frame");
		this.setBackground(Color.green);
		this.setLayout(null);
		this.addWindowListener(new WindowAdapter(){
			public void windowClosing(WindowEvent we){
				System.exit(0);
			}
		});
		
		b1=new Button("First");
		b2=new Button("Next");
		b3=new Button("Previous");
		b4=new Button("Last");
		
		b1.addActionListener(this);
		b2.addActionListener(this);
		b3.addActionListener(this);
		b4.addActionListener(this);
		
		Font f=new Font("arial",Font.BOLD,20);
		b1.setFont(f);
		b2.setFont(f);
		b3.setFont(f);
		b4.setFont(f);
		b1.setBounds(50,400,100,30);
		b2.setBounds(160,400,100,30);
		b3.setBounds(270,400,100,30);
		b4.setBounds(380,400,100,30);
		this.add(b1);
		this.add(b2);
		this.add(b3);
		this.add(b4);
		es=new EmployeeService();
	}
	public void actionPerformed(ActionEvent ae){
		label=ae.getActionCommand();
		eto=es.getEmployee(label);
		repaint();
	}
	public void paint(Graphics g){
		Font f=new Font("arial",Font.BOLD,30);
		g.setFont(f);
		String msg=es.getMsg();
		if(msg.equals("")){
			g.drawString("Employee Number  :"+eto.getEno(), 50, 100);
			g.drawString("Employee Name  :"+eto.getEname(), 50, 150);
			g.drawString("Employee Salary  :"+eto.getEsal(), 50, 200);
			g.drawString("Employee Address  :"+eto.getEaddr(), 50, 250);
			
		}else{
			g.drawString(msg, 50, 300);
		}
	}
	
}


EmployeeService.java

package jdbcApp17;
import java.sql.*;
public class EmployeeService {
	Connection con;
	Statement st;
	ResultSet rs;
	EmployeeTo eto;
	String msg="";
	boolean b=false;
	public EmployeeService(){
		try{
			Class.forName("oracle.jdbc.OracleDriver");
			con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
			st=con.createStatement(ResultSet.TYPE_SCROLL_INSENSITIVE,ResultSet.CONCUR_UPDATABLE);
			rs=st.executeQuery("select *from emp1");
		}catch(Exception e){
			e.printStackTrace();
		}
	}
	public EmployeeTo getEmployee(String label){
		try{
			if(label.equals("First")){
					rs.first();
					msg="";
		}
			if(label.equals("Next")){
				b=rs.next();
				if(b==false){
					msg="No More Records is Forward Direction";
				}else{
					msg="";
				}
			}
			if(label.equals("Previuos")){
				b=rs.previous();
				if(b==false){
					msg="No More Record In Background Direction";
				}else{
					msg="";
				}
			}
			if(label.equals("Last")){
				rs.last();
				msg="";
				
			}
			eto=new EmployeeTo();
			eto.setEno(rs.getInt(1));
			eto.setEname(rs.getString(2));
			eto.setEsal(rs.getFloat(3));
			eto.setEaddr(rs.getString(4));
	}catch(Exception e){
		e.printStackTrace();
	}
		return eto;
}
	public String getMsg(){
		return msg;
	}
	}

EmployeeTo.java
	
	
	package jdbcApp17;

public class EmployeeTo {
	private int eno;
	private String ename;
	private float esal;
	private String eaddr;
	public int getEno(){
		return eno;
	}
	public void setEno(int eno){
		this.eno=eno;
	}
	public String getEname(){
		return ename;
	}
	public void setEname(String ename){
		this.ename=ename;
	}
	public float getEsal(){
		return esal;
	}
	public void setEsal(float esal){
		this.esal=esal;
		
	}
	public String getEaddr(){
		return eaddr;
	}
	public void setEaddr(String eaddr){
		this.eaddr=eaddr;
	}
}

jdbcApp17.java


package jdbcApp17;

public class jdbcApp17 {

	public static void main(String[] args) {
		PlayerFrame pf=new PlayerFrame();
	}

}

**************************************************************

/* Scroll Sensitive ResultSet */
package jdbcApp18;
import java.sql.*;
public class jdbcApp18 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:ORCL","bipin","oracle");
		Statement st=con.createStatement(ResultSet.TYPE_SCROLL_INSENSITIVE,ResultSet.CONCUR_UPDATABLE);
		ResultSet rs=st.executeQuery("select *from emp1");
		System.out.println("Data Before Updation ");
		System.out.println("ENO    ENAME    ESAL    EADDR ");
		System.out.println("-----------------------------------");
		while(rs.next()){
			System.out.println(rs.getInt(1)+"\t"+rs.getString(2)+"\t"+rs.getFloat(3)+"\t"+rs.getString(4));
			
		}
		System.out.println();
		System.out.println("Application in pausing state ,please update database");
		System.in.read();
		rs.beforeFirst();
		System.out.println("Data after updation");
		System.out.println("ENO    ENAME    ESAL    EADDR ");
		System.out.println("-----------------------------------");
		while(rs.next()){
			System.out.println(rs.getInt(1)+"\t"+rs.getString(2)+"\t"+rs.getFloat(3)+"\t"+rs.getString(4));
			
		}
		System.out.println();
		con.close();
	}

}
************************************

/* PreparedStatemet example */
package jdbcApp22;
import java.sql.*;
public class jdbcApp22 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:orcl","bipin","oracle");
		PreparedStatement pst=con.prepareStatement("update emp1 set esal=esal+? where esal<? ");
		pst.setInt(1, 500);
		pst.setFloat(2, 100000.0f);
		int rowCount=pst.executeUpdate();
		System.out.println("Records Update :"+rowCount);
		con.close();
	}

}

***********************************

package jdbcApp23;
import java.sql.*;
public class jdbcApp23 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:orcl","bipin","oracle");
		PreparedStatement pst=con.prepareStatement("select *from emp1 where esal<?");
		pst.setFloat(1,7000.0f);
		ResultSet rs=pst.executeQuery();
		System.out.println("ENO   ENAME   ESAL   EADDR ");
		System.out.println("-------------------------------");
		while(rs.next()){
			System.out.println(rs.getInt(1)+"\t"+rs.getString(2)+"\t"+rs.getFloat(3)+"\t"+rs.getString(4));
			
		}
		con.close();
	}

}


**********************************

package jdbcApp24;
 import java.sql.*;
 import java.util.*;
public class jdbcApp24 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:orcl","bipin","oracle");
		PreparedStatement pst=con.prepareStatement("insert into std_course values(?,?,?,?)");
		pst.setString(1, "S-11");
		pst.setString(2, "bipin");
		pst.setString(3, "java");
		//Date d=Date.valueOf("2017-05-06");
		java.util.Date d=new java.util.Date();
		int val1=d.getDate();
		java.sql.Date d1=new java.sql.Date(val1);
		
		pst.setDate(4, d1);
		
		pst.executeUpdate();
		pst.setString(1, "S-22");
		pst.setString(2, "kumar");
		pst.setString(3, "oracle");
		java.util.Date date=new java.util.Date();
		int val=date.getDate();
		java.sql.Date dt=new java.sql.Date(val);
		
		pst.setDate(4, dt);
		
		pst.executeUpdate();
		
		con.close();
	}

}
***************************************

/* Batch updation */
package jdbcApp25;
import java.sql.*;
public class jdbcApp25 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:orcl","bipin","oracle");
		Statement st=con.createStatement();
		st.addBatch("insert into emp1 values(1003,'daya',5000,'bgp')");
		st.addBatch("update emp1 set esal=esal+500 ");
		st.addBatch("delete from emp1 where esal<4000");
		//st.addBatch("select *from emp1");//exception rise
		int[] rowCount=st.executeBatch();
		for(int i=0;i< rowCount.length;i++){
			System.out.println("Record manipulate :"+rowCount[i]);
		}
		con.close();
	}

}

************************************

/* batch updation using PreparedStatement */
package jdbcApp26;
import java.sql.*;
public class jdbcApp26 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:orcl","bipin","oracle");
		PreparedStatement pst=con.prepareStatement("insert into emp1 values(?,?,?,?)");
		pst.setInt(1,1006);
		pst.setString(2, "sant");
		pst.setFloat(3, 5000);
		pst.setString(4, "bgp");
		pst.addBatch();
		
		pst.setInt(1,1007);
		pst.setString(2, "santosh");
		pst.setFloat(3, 5000);
		pst.setString(4, "bgp");
		pst.addBatch();
		int[] rowCount=pst.executeBatch();
		for(int i=0;i<rowCount.length;i++){
			System.out.println("Records manipulation :"+rowCount[i]);
		}
		con.close();
	}

}

************************************



/* use savePoint */
package jdbcApp29;
import java.sql.*;
public class jdbcApp29 {

	public static void main(String[] args) {
		Connection con=null;
		try{
		   Class.forName("oracle.jdbc.OracleDriver");
		   con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:orcl","bipin","oracle");
		   con.setAutoCommit(false);
		   Statement st=con.createStatement();
		   st.executeUpdate("insert into student values(1005,'neeraj','bgp')");
		   Savepoint sp=con.setSavepoint();
		   st.executeUpdate("insert into student values(1006,'bipiin','bgp')");
		   con.rollback();
		   st.executeUpdate("insert into student values(1007,'kumar','bgp')");
		   con.commit();
		   System.out.println("Transaction success ");
		   
		
		}catch(Exception e){
		      try{
		    	  con.rollback();
		    	  System.out.println("Transaction failed ");
		      }catch(Exception e1){
		    	  e1.printStackTrace();
		      }
		}
	}

}

**********************************

CALLABLE STATEMENT 

create or replace procedure getSal(id in number,sal out number)
as
begin
select esal into sal from emp1 where eno=id;
end getSal;

/* use calaabale staement   first create procedure getSal*/
package jdbcApp30;
import java.sql.*;
public class jdbcApp30 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:orcl","bipin","oracle");
		CallableStatement cst=con.prepareCall("{call  getSal(?,?)}");
		cst.setInt(1, 1001);
		cst.registerOutParameter(2, Types.FLOAT);
		cst.execute();
		System.out.println("Salary = "+cst.getFloat(2));
	}

}
*********************************





package jdbcApp32;
import java.sql.*;
import java.io.*;
import java.util.Properties;
import oracle.jdbc.internal.OracleTypes;
public class jdbcApp32 {

	public static void main(String[] args)throws Exception {
		FileInputStream fis=new FileInputStream("db.properties" );
		Properties p=new Properties();
		p.load(fis);
		String driver_class=p.getProperty("driver_class");
		String driver_url=p.getProperty("driver_url");
		Class.forName(driver_class);
		Connection con=DriverManager.getConnection(driver_url,p);
		CallableStatement cst=con.prepareCall("{ call getEmps(?,?)}");
		cst.setFloat(1, 10000);
		cst.registerOutParameter(2, OracleTypes.CURSOR);
		cst.execute(); 
	    Object obj=cst.getObject(2);
	    ResultSet rs=(ResultSet)obj;
	    System.out.println("ENO \t ENAME \t ESAL \t EADDR");
	    System.out.println("----------------------------------");
	    while(rs.next()){
	    	System.out.println(rs.getInt(1)+"\t"+rs.getString(2)+"\t"+rs.getFloat(3)+"\t"+rs.getString(4));
	    }
	    rs.close();
	    con.close();
	}

}

/*
create or replace procedure getEmps(sal in number,emps out sys_refcursor)
as
begin
open emps for
select *from emp1 where esal<sal;
end getEmps;
*/

output give in db.properties file 

************************************



/* Connection pooling */
package jdbcApp33;
import java.sql.*;
import javax.sql.*;
import oracle.jdbc.pool.*;
public class jdbcApp33 {

	public static void main(String[] args)throws Exception {
		//prepare DataSource object
		OracleConnectionPoolDataSource ds=new OracleConnectionPoolDataSource();
		//set the parameters 
		ds.setURL("jdbc:oracle:thin:@localhost:1521:orcl");
		ds.setUser("bipin");
		ds.setPassword("oracle");
		//get pooledConnection object
		PooledConnection pc=ds.getPooledConnection();
		//get connection object from pooledConnection
		Connection con=pc.getConnection();
		//prepare statement
		Statement st=con.createStatement();
		ResultSet rs=st.executeQuery("select *from emp1 order by 1");
		System.out.println("EID    ENAME    ESAL ");
		System.out.println("-------------------------");
		while(rs.next()){
			System.out.println(rs.getInt(1)+"\t"+rs.getString(2)+"\t"+rs.getFloat(3));
		}

	}

}


*********************************

/* blob */
package jdbcApp34;
import java.sql.*;
import java.io.*;
public class jdbcApp34 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:orcl","bipin","oracle");
		File f= new File("blogo.png");
		FileInputStream fis=new FileInputStream(f);
		PreparedStatement pst=con.prepareStatement("insert into emp_details values(?,?,?)");
		pst.setInt(1,1001);
		pst.setString(2,"bipin's logo");
		pst.setBinaryStream(3, fis,(int)f.length());
		pst.executeUpdate();
		System.out.println("Employee Image inserted Successfully ");
		con.close();

	}

}



********************************

 /* retrive blob type data*/
package jdbcApp35;
import java.sql.*;
import java.io.*;
public class jdbcApp35 {

	public static void main(String[] args)throws Exception {
		Class.forName("oracle.jdbc.OracleDriver");
		Connection con=DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:orcl","bipin","oracle");
		Statement st=con.createStatement();
		ResultSet rs=st.executeQuery("select *from emp_details");
		rs.next();
		System.out.println("Employee id :"+rs.getInt(1));
		System.out.println("Employee Name :"+rs.getString(2));
		InputStream is=rs.getBinaryStream(3);
		FileOutputStream fos=new FileOutputStream("blogo.png");
		int i=is.read();
		while(i!=-1){
			fos.write(i);
			i=is.read();
		}
		System.out.println("Image create Successfully with the name blogo.png");
		fos.close();
		con.close();

	}

}


*******************************
