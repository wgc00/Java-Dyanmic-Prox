
 * IoC主要做两件事：把对象初始化后放入容器中。
 * 任何通过getBean()获取值
 
 ### 代理模式
 * 一般来说我们不使用继承，因为他会获得额外的功能。
 * 那我们使用什么呢？ 组合，组合（代理模式）优于继承
 
 * 动态的代理是：  
       好处：很简单  
       缺点： 这里类要基于接口，才能实现动态代理   
       如果没有接口的类呢？出现了第三方夹包  
       如： CGLib
       
       
 * 代理： 功能切割（因为重复）
 
 * jdb代理：灵活、可以单独代理、也可以多重代理  
    缺点： 必须有接口  
    
 * cglib代理： 不使用接口  
    缺点： 是对class文件在进行字符编码修改
    
    
 * 数据连接：
    一般情况下我们关闭Connection.close(), Statement.close()是会自动关闭的，
    如果是调用线程池Statement是不会关闭的，它会放到连接池
    
    Statement.close()的关闭的时, ResultSet也会关闭的，但
    ResultSet是在java虚拟机处理垃圾回收才把那个对象给清理，
    java的清理是不确定性的，如果对象过多就会报一个连接Cursor过多的错误
    
  
    
    
晚上作用：
    Controller包下  
    + user  
    + book  
    + admin  
    权限控制：登陆
    
    
    原子性：要全成功，要不成功
    一致性：两个人同时操作一个数据时，怎么保证这个数据不会报错，
    隔离性：
    耐久性：