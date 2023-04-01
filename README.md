# -
Работа на 4.03

fun main(args: Array<String>) {
    val number: Int = 27
    println("Входит ли в число $number цифра 7?")
    if (number/10==7 || number%10==7)
    println ("Да")
    else 
    println ("Нет")
}

fun main(args: Array<String>) {
    val number: Int = 27
    println("Входит ли в число $number цифра 7?")
    if (number/10==7 || number%10==7)
    println ("Да")
    else 
    println ("Нет")
}

fun main(args: Array<String>) {
    val number: Int = 22
    val a: Int = 1
    val b: Int = 15
    println("Принадлежит ли число $number диапазону [$a;$b]?")
    if (number>=a && number <=b)
    println ("Да")
    if (!(number>=a && number <=b))
    println ("Нет")
}

fun main(args: Array<String>) {
    val number: Int = 90
    if (number < 1000000 && number > 0)
    print ("Сумма заказа: $number")
    else
    println("Неверно указана сумма заказа")
    if(number%10==1)
    println(" рубль")
    if(number%10==2 || number%10==3  || number%10==4)
    println(" рубля")
    if(number%10==5 || number%10==6  || number%10==7 || number%10==8 || number%10==9 || number%10==0)
    println(" рублей")
}

fun main(args: Array<String>) {
    val age: Int = 25
    val SNP = "Товарищ Лутягин"
    val gender = "мужской"
    if (age<18)
    println("Клиент не достиг возраста совершеннолетия.")
    else
    when (gender) {
        "мужской" -> print("Уважаемый ")
        "Мужской" -> print("Уважаемый ")
        "женский" -> print("Уважаемая ")
        "Женский" -> print("Уважаемая ")
    }
	print (SNP)
	if (age>=18 && !(age%10==0 || age%10==5))
    print("Поздравляю вас с Днем Рождения.")
    if (age%10==0 || age%10==5)
    print(", поздравляю вас с Юбилеем.")
   	print(" От лица нашей компании желаю вам всего самого наилучшего.")
}

Вопрос:

fun main(args: Array<String>) {
    val age: Int = 25
    val SNP = "Товарищ Лутягин"
    val gender = "мужской"
    if (age<18)
    println("Клиент не достиг возраста совершеннолетия.")
    else
    when (gender) {
        "мужской" -> print("Уважаемый ")
        "Мужской" -> print("Уважаемый ")
        "женский" -> print("Уважаемая ")
        "Женский" -> print("Уважаемая ")
    }
	print (SNP)
	if (age>=18 && !(age%10==0 || age%10==5))
    print("Поздравляю вас с Днем Рождения.")
    if (age%10==0 || age%10==5)
    print(", поздравляю вас с Юбилеем.")
   	val i1 = "Наша фирма желает вам долголетия."
    val i2 = "Наша фирма желает вам крепкого здоровья."
    val i3 = "Наша фирма желает вам всех благ."
    val random = arrayOf(i1,i2,i3)
    print(random)
}
//Уважаемый Товарищ Лутягин, поздравляю вас с Юбилеем.[Ljava.lang.String;@20ad9418
Чем может быть [Ljava.lang.String;@20ad9418 ?
	
	
	задачи по теме 3 и 4
	
	package kotlin.math

fun main() {
    var A = 2.0
    var B = 4.0
    var a = false
    var b = false
    var B1 = B.pow(3.0)
    var A1 = A.pow(3.0)

    if (A<B) {
    do {
        var C = A.pow(3.0)
        print("$C; ")
        A++
        if (A == B)
            a = true
    } while (!a)
    print("$B1")
    }
    else {
     (A>B)
    do {
        var C1 = B.pow(3.0)
        print("$C1; ")
        B++
        if (B == A)
            b = true
    } while (!b)
    print("$A1")
    }
}
	
	
	package kotlin.math

fun main() {
    var n1 = 0.0
    var n2 = 1.0
    var i = 2.0
    var N = 10.0
    var I = false
    
    print("$n1; $n2; ")
  	if (i<N) {
       do {
       var sum = n1 + n2
           print("$sum; ")    
       n1 = n2 ;
       n2 = sum
       i++
       if (i == N)
       I = true  
   } while(!I)
   }
}
		 
 package kotlin.math

fun main() {
    var num = 9044
    var revers = 0
    
    while (num != 0) {
        val number = num % 10
        revers = revers * 10 + number
        num /= 10    
    }
    println("$revers")
}
		 
fun main() {
	var num = 13573
    var N = 3
    
          while (num != 0) {
              val number = num % 10
              if (number == N) {
                      print("")
                  }
              else {
                  print("$number")
              }
              num /= 10
              }   
          } //не хватило терепения на переворачивание обратно
		 
fun main() {
	var A: Int = 146
    var a = false
    
    if (A / 2 == 0) {
        do {
            var AA = A / 2
            if (A==1)
            	a = true
        } while (!a)
        println(A)
    }
  	else  {
        do {
        var AB = A * 3
        var sum = AB + 1
        var Aa = sum / 2
            if (A==1)
            	a = true
    } while (!a)
        println(A)
    }
          } //кажется, что оно где-то рядом с правдой, но выдает Evaluation stopped while it's taking too long️
		
		
fun main() {
	val man: Person = Person()
    val man2: Person  = Person(_fullName = "Некто") 

    println(man2.fullName)
    
    man.fullName = "Товарищ Летягин"
	man.age = 20   

	println(man.fullName)
    println(man.age)

	man.move()
    man.talk()
	
}

class Person() {
    val fullName: String = "Отсутствует"
    val age: Int = 18
    
    fun move() {
        print("Идет и ")
    }
    
    fun talk() {
        println("такой-то Person говорит")
    }
    
class Person(_fullName: String) {
    val fullName: String 
    
    
    init {
        fullName = _fullName
    }
} 
}
	
	fun main() {
      
    class Engine{
    	val power: Int = 1
    	val manufacturer: String = "Отсутствует"
    }
    class Driver{
        val FIO: String = "Отсутствует"
        val stag: Double = 1.2
    }
    open class Car{
    	val name: String = "Отсутствует"
    	val tipe: String = "A"
    	val weight: Double = 1.5
    	val man: Driver = Driver()
    	val motor: Engine = Engine()
    
    	fun start(){
            println("Поехали")
        }
    	fun stop(){
            println("Останавливаемся")
        }
    
    	fun turnRight(){
            println("Поворот направо")
        }
    	fun turnLeft(){
            println("Поворот налево")
        
   		fun toString(){
            
            println("Авто: $name; $tipe; $weight; $man; $motor")
        }
        
        class Lorry : Car() {
            val loadCapacity: Double = 1.75
        }
        class SportCar : Car() {
            val MaxSpeed: Int = 220
        }
        }
    }
    }
	
	
	
