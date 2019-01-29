# Java-Dyanmic-Prox
设计模式之代理模式，明天上传


main方法中使用对象AnnotationConfigApplicationContext往容器中注入配置对象
    
       AnnotationConfigApplicationContext context = new AnnotationConfigApplicationContext(SpringDAOConfig.class);
        SQLStatement bean = context.getBean(SQLStatement.class);
        try {
            bean.add("dd");
        } catch (SQLException e) {
            e.printStackTrace();
            System.out.println("报错");
        }


## 代理模式

  理念[https://github.com/wgc00/Java-Dyanmic-Prox/blob/master/src/main/java/notes/Spring.md]
