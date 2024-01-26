```java
/**
 * @author Dmytro Liashenko
 * @location Kyiv, Ukraine
 * @email dmitriy.lyashenko.java@gmail.com
 * @phone (095) 812-57-80
 * @bio Experienced and creative developer with 7+ years of experience in project planning, implementation and
 * implementation in various areas of software. I am looking for opportunities for development, gaining new experience
 * and ready to learn new technologies. I prefer projects starting "from scratch"
 * and projects related to the field of artificial intelligence.
 */
@JavaDeveloper
public class CV {

    public enum SoftSkils {
        Java, JavaFx, JavaScript, TypeScript, SQL, Spring(Boot, Web, MVC, Data, Security, AOP, Batch),
        Postgres, H2, IoC, SOLID, Docker, Kubernetes, Maven,  Liquibase, Hibernate, JDBC, JSP, JPA,
        JSON, XML, CSV, HTML, Freemarker, Thymeleaf, Selenium, Nginx, SLF4J, JWT, Git, GitHub, GitLab,
        Jenkins, Intellij IDEA, REST APIs, Swagger, Restful Web Services, JHipster, JUnit, Mockito,
        Angular, React
        }

    static class WorkExpirience implements Projects {

        public final static String company = "Corside Group";
        public final static String position = "Java Developer";
        public final static WorkRange workRange =  new WorkRange(Month.SEPTEMBER, 2017, Month.JANUARY, 2024);

        @Override
        public List<Project> projetes() {
            return Stream.of(
                    new Project("Tyresnet / www.tyres.net", new WorkRange(Month.MARCH, 2021, Month.JANUARY, 2024),
                            "Marketplace for tires and wheels. I joined a multi-module and diverse technological project " +
                                    "where my main responsibilities were improving the existing one, implementing " +
                                    "new functionalities, correcting errors and refactoring the code."),
                    new Project("VA Recoredr", new WorkRange(Month.MARCH, 2020, Month.APRIL, 2021),
                            "The VA Recoredr project is a cross-platform desktop application for video and audio capture, " +
                                    "event logging, and the ability to transfer saved data to external media. Participated in " +
                                    "all stages of development. The main responsibility was the implementation of the above " +
                                    "functionality, as well as the implementation of the administration, licensing and " +
                                    "product update server."),
                    new Project("Patyment Methon", new WorkRange(Month.MARCH, 2019, Month.APRIL, 2020),
                            "Took part in all stages of project creation for some banks with limited access to internet banking."),
                    new Project("Reifentest / www.reifentest.com", new WorkRange(Month.NOVEMBER, 2018, Month.MARCH, 2019),
                            "A portal for collecting tire reviews. I joined a project where my task included improving " +
                                    "existing functions, fixing errors and refactoring the code."),
                    new Project("Paymeent Gateway", new WorkRange(Month.SEPTEMBER, 2017, Month.SEPTEMBER, 2018),
                            "Participated in all stages of development, starting from the concept to its successful " +
                                    "implementation. The main responsibility was the development of the \"core\", which included " +
                                    "the implementation of another payment gateway's API and the creation of its own API with " +
                                    "the possibility of integrating direct payment methods. In addition, he participated in " +
                                    "the development and implementation of the administrative interface, which included " +
                                    "the management and monitoring of payment transactions, etc.")
                            .toList();
        }
    }

    public static String courses() {
        return "DevOps basics, “Prometheus”\n" +
                "English Pre-Intermediate, “Green Forest”\n" +
                "Java programming, “JuJa”\n" +
                "Java programming, “IT-Center”\n"
    }

    @Ukrainian("native")
    @English("intermediate")
    public static String education() {
        return "Donetsk National Technical University\n" +
                "Specialist, Enterprise management 2006 - 2010\n" +
                "Donetsk National Technical University\n" +
                "Control and automation systems 2004 - 2006\n"
    }
}
```
  
