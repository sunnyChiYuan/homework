import java.util.Scanner;
public class Main {  
    public static void main(String args[]){
        Scanner i=new Scanner(System.in);
        printMenu();
        int SelsctItem = i.next();
        voitMenu(SelsctItem);
    }
    //顯示系統功能
    public static void printMenu() {  
        System.out.println("\n========== 線上投票系統 ==========");
        System.out.println("1. 顯示所有投票項目");
        System.out.println("2. 選擇投票項目");
        System.out.println("3. 新增投票項目");
        System.out.print("請選擇功能：");
    }
    //篩選輸入者選擇的項目
    public static void voitMenu(int choice)
    {
        switch (choice) {
                case "1":
                    showAllVotes();
                    break;
                case "2":
                    choiceVoteItem();
                    break;
                case "3":
                    addVoteItem();
                    break;               
                default:
                    System.out.println("系統結束。");
            }
    }
    //顯示投票項目
    public static void showAllVotes(){
        System.out.println("1. 電腦");
        System.out.println("2. 滑鼠");
    }
     //投票人選擇投票項目
    public static void choiceVoteItem(){
        Scanner n=new Scanner(System.in);
        Scanner m=new Scanner(System.in);
        System.out.println("填入您的(投票人)名字:");
        char voterName = n.next();
        System.out.println("您要投票的編號:");
        char voterChoiceItem = n.next();
    }
    //新增投票項目
    public static void addVoteItem(){


    }


}

