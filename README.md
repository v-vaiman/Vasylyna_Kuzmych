#  Homework for Java Lecture #3: Spring Intro & Core (Part 2)
###Java-based Container Configuration
1.	Підготувати 6-ть різних POJO класів для створення бінів, з обов\`язковими полями name, value та методом toString(). Назви бінів: `BeanA`, `BeanB`, `BeanC`, `BeanD`, `BeanE`, `BeanF`.
2.	Біни `BeanB`, `BeanC`, `BeanD` свої значення отримують з *.properties файлу
3.	Створити два файли конфігурації `@Configuration`, та імпортувати одну конфігурацію в іншу.
4.	Забезпечити такий порядок створення бінів: `BeanD`, `BeanB`, `BeanC`
5.	Забезпечити конфігурування біна `BeanF` з `@Lazy` ініціалізацією.
6.	При конфігуруванні бінів `BeanB`, `BeanC`, `BeanD` за допомогою `@Bean` анотації, задати назви користувацьких методів для атрибутів initMethod та destroyMethod, в яких виводити відповідні повідомлення.
7.	Бін `BeanA` повинен реалізовувати інтерфейси InitializingBean та DisposableBean. Перебачити відповідні повідомлення з реалізованих методів.
8.	Бін `BeanE` повинен мати методи з анотаціями `@PostConstruct` та `@PreDestroy`. Перебачити відповідні повідомлення з цих методів.
9.	Вивести перелік усіх бінів, що створені у ApplicationContext. Проаналізувати результати.
10.	Створити окремий бін, що реалізовує BeanFactoryPostProcessor. За допомогою нього для біна `BeanB` змінити параметр initMethod на значення іншого користувацького методу. Передбачити вивід відповідних повідомлень.
11.	Створити окремий бін, що реалізовує BeanPostProcessor. За допомогою нього здійснити валідацію наших бінів. Усі поля name повинні містити значення (not null), а поля value містити лише додатні значення.
12.	Вивести конфігурацію усіх бінів на екран з використанням ApplicationContext.

