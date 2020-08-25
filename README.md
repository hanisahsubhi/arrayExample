# arrayExample
Demo

class Main {
  public static void main(String[] args) {
    System.out.println("Hello world!");

    
    //create an array
    int axX [] = new int[3];
    axX[0] = 100;
    axX[1] = 200;
    axX[2] = 300;


    //access the array elements using For loop
    for (int x; x < axX.length; x ++){
      System.out.println(axX[x]);
    }
  }
}

//Bank Account. To have data of name & account number, stored using Array. Method to set data and to display information
class Account {
  String name;
  Long accountNum;

  //have two separate methods: 1.setting the data 2.display information
  void setData(String name, Long accountNum){
    this.name = name;
    this.accountNum = accountNum;
  }

  void display(){
    System.out.println("Name:" + name);
    System.out.println("Account Number:"+accountNum);
  }

  //declare array (type Account) restricting to size of 3
  Account arrAccount [] = new Account [3];
  //create object of an array, followed by setting a data for each object
  arrAccount[0] = new Account();
  arrAccount[0].setData("Waqiah", 1293929);

  arrAccount[1] = new Account();
  arrAccount[1].setData("Syeer", 134222222);

  arrAccount[2] = new Account();
  arrAccount[2].setData("Shiew", 829333921);
  

  //display infos using enhanched loop method
  System.out.println("These are the account infos:");
  for (Account account : arrAccount){
    account.display();
  }
}
}
