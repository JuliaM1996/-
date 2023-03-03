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
