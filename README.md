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
