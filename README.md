333333# codngProgrmJava
QUESTIONS
1. Number grater than 100
   2.Letter start with letter m
   3.even and odd number in data
    4.square of numbers
   5.add 5 to all numbers
   6. connvet ever letterss  to upper case annd lter LowerCase
   7. length of String
   8. Sort the record
   9.Remove duplicate
10.Names with length more than four
11.Filter names starts with "J" convert to Uppercase & collect

Test attempts/Tranning/practice
January/2026
sl   :  Date      : Time     : no_of_Time/practice    : TimeTaken/Duration  : TotalQuestons :Questionn _Number : QuestionnTpe
1    :                                                                                                          :Basic
2    :            :          :    2                   :   ≈40 min           :  11q           : 1 to 11           :  Basic
3    : 18/01/2026 : 1:36am   :    3                   :    32.05 min        :  11q            : 1 to 11          :Basic    
3


Programs

1. Number grater than 100

   public static void main(String[] args) {

        List<Integer> data = Arrays.asList(100, 351015, 500, 700);
        List<Integer> newData=data.stream().filter(x->x>100).collect(Collectors.toList());
        System.out.println(newData);

    }

   2.Letter start with letter m

    public static void main(String[] args) {

        List<String> data = Arrays.asList("mike","adam","madam","bik","me");
        List<String> newData=data.stream().filter(x->x.startsWith("m")).collect(Collectors.toList());
        System.out.println(newData);

    }

3.even and odd number in data

   public static void main(String[] args) {

        List<Integer> data = Arrays.asList(10,11,013,14,16,19);
        List<Integer> newData=data.stream().filter(t->t%2==0 ).collect(Collectors.toList());
        System.out.println("even ::  "+newData);

        List<Integer> data2 = Arrays.asList(10,11,013,14,16,19);
        List<Integer> newData2=data.stream().filter(t->t%2!=0 ).collect(Collectors.toList());
        System.out.println("odd ::  "+newData2);

    }

    4.square of numbers

    public static void main(String[] args) {

        List<Integer> data = Arrays.asList(10,11,013,14,16,19);
        List<Integer> newData=data.stream().map(x->x*x ).collect(Collectors.toList());
        System.out.println("square of numbers ::  "+newData);
        }

5.add 5 to all numbers

 public static void main(String[] args) {

        List<Integer> data = Arrays.asList(10,11,013,14,16,19);
        List<Integer> newData=data.stream().map(x->x+5 ).collect(Collectors.toList());
        System.out.println("add 5 to all numbers ::  "+newData);}

6. connvet ever letterss  to upper case annd lter LowerCase

    public static void main(String[] args) {

        List<String> list = Arrays.asList("deddLLLLSSSaaa","SSWWEEE","ssdd", "sssWWWW","WWWWWWeeee","AAAAAS","sss");
        List<String> collect = list.stream().map(x -> x.toUpperCase() ).collect(Collectors.toList());
        System.out.println("    " +collect );

7. length of String

 
        List<String> list = Arrays.asList("111","48","ssdd", "55","a","AAAAAS","sss");
        List<Integer> collect = list.stream().map(x -> x.length() ).collect(Collectors.toList());
        System.out.println("    " +collect );
        

8. Sort the record

List<String> list = Arrays.asList("111","48","ssdd", "55","a","AAAAAS","sss");
        List<String> collect = list.stream().sorted().collect(Collectors.toList());
        System.out.println("    " +collect );
        
9.Remove duplicate
List<String> list = Arrays.asList("111","48","1","sss","1","4","1");
        List<String> collect = list.stream().distinct().collect(Collectors.toList());
        System.out.println("    " +collect );

10.Names with length more than four

 List<String> list = Arrays.asList("14411","48","1","sss","1","4","1");
        List<String> collect = list.stream().filter(x->x.length()>4).collect(Collectors.toList());
        System.out.println("    " +collect );

11.Filter names starts with "J" convert to Uppercase & collect

List<String> list = Arrays.asList("14411","JJJ","JJJJ",  "J1","jsss","1","4","1","jLLL");
        List<String> collect = list.stream().filter(s->s.startsWith("j") ).map(String::toUpperCase).collect(Collectors.toList());
        System.out.println("    " +collect );

        List<String> list1 = Arrays.asList("14411","JJJ","JJJJ",  "J1","jsss","1","4","1");
        List<String> collect1 = list1.stream().filter(s->s.startsWith("j") ).map(l->l.toUpperCase()).collect(Collectors.toList());
        System.out.println("    " +collect1 );



 

        
        
