# codngProgrmJava

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


        
        
