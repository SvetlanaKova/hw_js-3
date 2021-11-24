// 1. Запросить у пользователя его возраст и определить, кем он 
// является: ребенком (0–2), подростком (12–18), взрослым 
// (18_60) или пенсионером (60– ...).

// const age = prompt("возраст");

// if (age <= 2 && age >= 0) {
// 	alert("ребенком");
// } else if (age >= 12 && age < 18) {
// 	alert("подростком")
// } else if (age >= 18 && age <= 60) {
// 	alert("взрослым");
// } else if (age > 60) {
// 	alert("пенсионером");
// }


// 2. Запросить у пользователя число от 0 до 9 и вывести ему 
// спецсимвол, который расположен на этой клавише (1–!, 
// 2–@, 3–# и т. д).

// const char = prompt("число");

// switch (char) {
// 	case "1":
// 		alert("!");
// 		break;
// 	case "2":
// 		alert("@");
// 		break;
// 	case "3":
// 		alert("#");
// 		break;
// 	case "4":
// 		alert("$");
// 		break;
// 	case "5":
// 		alert("%");
// 		break;
// 	case "6":
// 		alert("^");
// 		break;
// 	case "7":
// 		alert("&");
// 		break;
// 	case "8":
// 		alert("*");
// 		break;
// 	case "9":
// 		alert("(");
// 		break;
// }

// 3. Запросить у пользователя трехзначное число и проверить, 
// есть ли в нем одинаковые цифры.

// let number = prompt("трехзначное число");

// let firstChar = (number % 10); // 321 - 1
// number = number / 10 | 0 // отбрасываем одно число - 32
// let secondChar = (number % 10); // 32 - 2
// let thirdChar = number / 10 | 0 // отбрасываем одно число - 3

// alert(`${firstChar} + ${secondChar} + ${thirdChar}`);


// if (firstChar == secondChar || secondChar == thirdChar) {
// 	alert("есть одинаковые цифры");
// } else if (secondChar == thirdChar && firstChar == secondChar) {
// 	alert("есть одинаковые цифры");
// } else {
// 	alert("нет одинаковых цифр");
// }

// 4. Запросить у пользователя год и проверить, високосный он 
// или нет. Високосный год либо кратен 400, либо кратен 4 и 
// при этом не кратен 100.

// let year = prompt("год");

// if (year % 400 == 0) {
// 	alert("високосный");
// } else if (year % 4 == 0 && !(year % 100 == 0)) {
// 	alert("високосный");
// } else {
// 	alert("не високосный");
// }


// 5. Запросить у пользователя пятиразрядное число и опреде-
// лить, является ли оно палиндромом.

// let number = prompt("пятиразрядное число");

// let temp = number;

// let firstChar = (number % 10) * 10000; // 12321 - 1
// number = number / 10 | 0 // отбрасываем одно число - 1232
// let secondChar = (number % 10) * 1000; // 1232 - 2
// number = number / 10 | 0 // отбрасываем одно число - 123
// let thirdChar = (number % 10) * 100; // 123 - 3
// number = number / 10 | 0 // отбрасываем одно число - 12
// let fourthChar = (number % 10) * 10; // 12 - 2
// let fifthChar = number / 10 | 0 // отбрасываем одно число - 1


// let reversNumber = firstChar + secondChar + thirdChar + fourthChar + fifthChar;

// if (temp == reversNumber) {
// 	alert("палиндром");
// } else {
// 	alert("нет");
// }

// 6. Написать конвертор валют. Пользователь вводит количе-
// ство USD, выбирает, в какую валюту хочет перевести: EUR, 
// UAN или AZN, и получает в ответ соответствующую сумму.

// let dollarsCount = prompt("количество USD");
// let currency = prompt("в какую валюту хочет перевести");

// const euroPerDollars = 0.88574;
// const uanPerDollars = 0.1567;
// const aznPerDollars = 0.58861;

// if (currency == "USD") {
// 	alert(dollarsCount * euroPerDollars);
// } else if (currency == "UAN") {
// 	alert(dollarsCount * uanPerDollars);
// } else if (currency == "AZN") {
// 	alert(dollarsCount * aznPerDollars);
// }

// 7. Запросить у пользователя сумму покупки и вывести сумму 
// к оплате со скидкой: от 200 до 300 – скидка будет 3%, от 300 
// до 500 – 5%, от 500 и выше – 7%. 

// let sum = prompt("сумму покупки");

// if (sum > 200 && sum < 300) {
// 	let total = sum - (sum * 3 / 100);
// 	alert(`сумму к оплате со скидкой: ${total}`)
// } else if (sum > 300 && sum < 500) {
// 	let total = sum - (sum * 5 / 100);
// 	alert(`сумму к оплате со скидкой: ${total}`)
// } else if (sum > 500) {
// 	let total = sum - (sum * 7 / 100);
// 	alert(`сумму к оплате со скидкой: ${total}`)
// }

// 8. Запросить у пользователя длину окружности и периметр 
// квадрата. Определить, может ли такая окружность поме-
// ститься в указанный квадрат. 

// const piNumber = 3.14;

// let circleLength = prompt("длину окружности");
// let squarePerimeter = prompt("периметр квадрата");

//диаметр через длину окружности
// let circleDiameter = circleLength / piNumber; 

// длина стороны квадрата
// let squareLength = squarePerimeter / 4; 

// Круг уместится в квадрат только тогда, когда его диаметр будет
// не больше стороны квадрата:

// if (squareLength > circleDiameter) {
// 	alert("может");
// } else {
// 	alert("не может");
// }

// 9. Задать пользователю 3 вопроса, в каждом вопросе по 3 ва-
// рианта ответа. За каждый правильный ответ начисляется 2 
// балла. После вопросов выведите пользователю количество 
// набранных баллов.

// let firstQuestion = prompt("1 вопрос");
// let secondQuestion = prompt("2 вопрос");
// let thirdQuestion = prompt("3 вопрос");

// if (firstQuestion == 2) {
// 	firstQuestion = true;
// } else firstQuestion = false;
// if (secondQuestion == 3) {
// 	secondQuestion = true;
// } else secondQuestion = false;
// if (thirdQuestion == 1) {
// 	thirdQuestion = true;
// } else thirdQuestion = false;

// let score = 0;

// if (firstQuestion) {
// 	score = score + 2;
// }
// if (secondQuestion) {
// 	score = score + 2;
// }
// if (thirdQuestion) {
// 	score = score + 2;
// }
// alert(score);

// 10.  Запросить дату (день, месяц, год) и вывести следующую 
// за ней дату. Учтите возможность перехода на следующий 
// месяц, год, а также високосный год. 

let someDate = prompt("Запросить дату (день, месяц, год)"); // формат даты: 23.11.2021

let someDay = someDate.slice(0,2); // 23
let someMonth = someDate.slice(3,5); // 11
let someYear = someDate.slice(6); // 11

alert(`Первоначальный вариант: ${someDay}.${someMonth}.${someYear}`);

// проверить, високосный он 
// или нет. Високосный год либо кратен 400, либо кратен 4 и 
// при этом не кратен 100.
let leapYear;
if (someYear % 400 == 0) {
	leapYear = someYear;
} else if (someYear % 4 == 0 && !(someYear % 100 == 0)) {
	leapYear = someYear;
} 

if (someDay == 28 && someMonth == 02 && someYear == leapYear) {
	someDay = 29;
}
if (someDay == 29 && someMonth == 02 && someYear == leapYear) {
	someDay = "01";
	someMonth = "03";
}

if (someDay <= 30 && (someMonth == 01 || someMonth == 03 || someMonth == 05 || someMonth == 07 || someMonth == 08 || someMonth == 10 || someMonth == 12)) { 
	someDay = +someDay + 1;
}
if (someDay == 30 && (someMonth == 02 || someMonth == 04 || someMonth == 06 || someMonth == 09 || someMonth == 11)) { 
	someDay = "01";
	someMonth = +someMonth + 01;
}
if (someDay == 31 && (someMonth == 01 || someMonth == 03 || someMonth == 05 || someMonth == 07 || someMonth == 08 || someMonth == 10)) { 
	someDay = "01";
	someMonth = +someMonth + 01;
}
if (someDay == 31 && someMonth == 12) { 
	someDay = "01";
	someMonth = "01";
	someYear = +someYear + 01;
}
if (someDay < 30) { 
	someDay = +someDay + 1;
}

alert(`Новая дата : ${someDay}.${someMonth}.${someYear}`);
