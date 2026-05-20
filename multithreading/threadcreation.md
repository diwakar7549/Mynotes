
Thread creation using runnable interface use this for real projects 

class mythread implements Runnable{
      
      public void run(){
         Syso("task");
      }

      public static void main(String[]args){

         mythread t = new mythread();
         thread th = new thread(t);
         th.start();
      }
}