
1.performing one task using one thread
2. performing multiple task using one thread
3. one thread multiple task not possible
4. multiple task multiple thread 
 
 example for multiple task multiple thread 
 
 class mythread1 extends thread{
     public void run(){
         Syso("task one ");
     }
 }

 class mythread2 extends thread{
    
    public void run(){
        syso("task two");
    }
 }

 class main{
    public static void main(String[]args){
        mythread1 t1 = new mythread1();
        t1.start();
        mythread2 t2 =  new mythread2();
         t2.start()
         <!-- i cannot comment one which one gets terminated first both are executed simultaneously
          -->
    }
 }