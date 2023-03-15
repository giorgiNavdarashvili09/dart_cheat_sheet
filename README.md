# Dart
დარტი კომპიუტერული პროგრამირების ენაა, რომელიც გამოიყენება ვებ-საიტების, მობულური აპლიკაციებისა და სხვა პროგრამების შესაქმნელად. დარტი გამოირჩევა მარტივი, თანამედროვე სინტაქსით და იდეალური არჩევანია დამწყებებისათვის.
### Code editors, DartPad
იმისათვის რომ დავიწყოთ Dart პროგრამირების ენის შესწავლა, ჩვენ გვჭირდება გავმართოთ "დეველოპმენტ გარემო" ჩვენს კომპიუტერებში. უფრო კონკრეტულად კი ჩვენ დაგვჭირდება:
- Dart sdk(**S**oftware **D**evelopment **K**it) არის დამხმარე ხელსაწყოებისა და ბიბლიოთეკების ერთობლიობა კომპიუტერული პროგრამების საწერად Dart ში
- Code Editor არის პროგრამა, რომელიც საშუალებას გვაძლევს დავწეროთ ან შესწორებები შევიტანოთ ჩვენი პროგრამების კოდში. კოდ ედიტორები სპეციალურად შექმნილია პროგრამული ენებისათვის და გვთავაზობს სხვადასხვა ხელსაწყოებს კოდის ეფექტურად წერისათვის. მაგ.: syntax hilighting(სინტაქსის "გაფერადება"), code completion(კოდის ფრაგმენტების აუტომატური დასრულება), debugging(კოდში შეცდომების/პრობლემების გამოსწორების პროცესი) და სხვა...
- Dart Plugin

ასევე ჩვენ შეგვიძლია გამოვიყენოთ [DartPad](https://dartpad.dev), რომელიც ონლაინ ედიტორია და Dart_ის საფუძვლების შესასწავლად სრულიად საკმარისია.

### Dart_ი Android Studio_ში
იმ შემთხვევაში თუ თქვენ გამართული გაქვთ თქვენი კომპიუტერი Flutter_ის აპლიკაციების საწერად, ჩვენ არ გვჭირდება Dart_ის ცალკე გადმოწერე. ჩვენ უბრალოდ უნდა ვუთხრათ ანდროიდ სტუდიოს სად არის Dart SDK. გახსენით Android Studio და შექმენით ახალი პროექტი New Flutter Project ღილაკის დახმარებით. მარცხენა მხარეს აირჩიეთ Dart, Dart SDK Path ველში აირჩიეთ შემდეგი მისამართი C:\src\flutter\bin\cache\dart-sdk. ამის შემდეგ ახალი პროექტის შექმნის ფანჯარა ასე უნდა გამოიყურებოდეს <br /><br />
<img src="/screenshots/new_project.png" ><br />
აირჩიეთ Next შემდეგ მიანიჭეთ პროექტს სახელი და create.

### Dart_ის პროექტი და ანდროიდ სტუდიოს ინტერფეისი
ახალი პროექტის შექმნის შემდეგ Android Studio დააგენერირებს საჭირო ფაილებსა და ფოლდერებს დარტის აპლიკაციისთვის.
Android Studio ავტომატურად გახსნის ფაილს, რომელშიც Dart_ის main ფუნქცია მოთავსებული. ფაილის სახელი შეესაბამება თქვენი პროექტის სახელს და მდებარეობს bin ფოლდერში. წაშალე ყველაფერი ამ ფაილში და შეიყვანე შემდეგი კოდი

```dart
    void main() {
        print("Hello, World!");
    }
```
გაუშვი პროექტი run ღილაკის დახმარებით ან shortcut_ით Shift + F10. თუ კი კონსოლში გამოვა მესიჯი "Hello, World!" მაშინ შენ წარმატებით შეძელი გარემოს გამართვა დარტის პროგრამების საწერად. ყველა მაგალითი, რომელსაც აქ განვიხილავთ შეგიძლია გატესტო ანდროიდ სტუდიოში, ხოლო მაგალითების უმეტესობის გასატესტად ასევე გამოდგება DartPad_ი.

### მონაცემთა ტიპები და ცვლადები.

მონაცემთა ტიპები და ცვლადები უმნიშვნელოვანესი კონცეფტებია პროგრამირებაში. მათი საშვალებით ჩვენ შეგვიძლია შევინახოთ და დავამუშაოთ სხვადასხვა ტიპის ინფორმაცია. დარტში გვხვდება სხვადასხვა მონაცემთა ტიპები (Data types).მაგალითად:<br />

1. Numbers: მოიცავს მთელ რიცხვებს (ინტეჯერი - int : 0,-3, 5, 23 ...) და ათწილადებს (double : 1.3, -23.23123 ....).
2. Strings: არის სიმბოლოების მიმდევრობა(ასოები, რიცხვები, სხვადასხვა ოპერატორები და ა.შ.)  და გამოიყენება ტექსტის გამოსახვისათვის.
3. Booleans: არის მონაცემის ტიპი რომელსაც შეუძლია მხოლოდ ორი მნიშვნელობის მიღება: true და false.
4. Lists: ეს არის ერთი და იგივე ტიპის ობიექტების კოლექცია

ცვლადი ეს არის კონტეინერი რომელშიც შეგვიძლია შევინახოთ სხვადასხვა მონაცემის ტიპის მნიშვნელობები. როდესაც ჩვენ ვქმნით ცვლადს, ჩვენ მას ვანიჭებთ სახელს - რომლის მეშვეობით, მოგვიანებით შევძლებთ იმ მნიშვნელობის წაკითხვას რაც შენახულია ცვლადში.

მოდით შევქმნათ ჩვენი პირველი ცვლადები მივანიჭოთ მათ სახელები და შევინახოთ გარკვეული ინფორმაცია მათში.

```dart
    var firstName = "გიორგი";
    var age = 27;
```

როგორც ხედავთ იმისათვის, რომ შევქმნათ ცვლადი ვიყენებთ var keyword_ს. var დარტს ეუბნება, რომ ჩვენ გვინდა ცვლადის შექმნა. ამის შემდეგ ჩვენს ცვლადს ვანიჭებთ სახელს. ცვლადის სახელი სასურველია იყოს ისეთი სიტყვა ან სიტყვათა შეთანხმება, რომელიც ნათლად აღწერს ინფორმაციას რომელსაც მასში შევინახავთ. ყურადღება მიაქციე რომ ცვლადის სახელში ყოველი სიტყვა გარდა პირველისა იწყება დიდი ასოთი. ამ მიდგომას პროგრამირებაში ეწოდება camelCase.

იმისათვის რომ დავინახოთ თუ რა ინფორმაცია შევინახეთ ცვლადებში, გამოვიყენებთ print() ფუნქციას.

```dart
    void main() {
    var firstName = "გიორგი";
    var age = 27;

    print(firstName);
    print(age);
    }
```

მიაქცი ყურადღება, რომ კოდი რომელიც ჩვენ დავწერეთ main ფუნქციის ფიგურულ ფრჩხილებშს შორის არის მოთავსებული.
ამ პროგრამის გაშვების შემდეგ კონსოლში გამოგვიჩნდება შესაბამისი მესიჯი<br /><br />
<img src="/screenshots/first_program.png" ><br />

```dart
  var firstName = "გიორგი";
```
მოდით გავარჩიეოთ ეს კოდის ფრაგმენტი:
- var : keyword_ს ვიყენებთ როდესაც გვინდა შევქმნათ ცვლადი მისი მონაცემის ტიპის მითითების გარეშე.
- firstName : არის ცვლადის სახელი. ცვლადის სახელი შეიძლება იყოს ლათინური ასოების და ციფრების კომბინაცია. თუმცა არ შეიძლება დაიწყოს ციფრით.
- = : უდრის სიმბოლოს ვიყენებთ იმისათვის რომ ჩვენს ცვლადს firstName_ს მივანიჭოთ მნიშვნელობა
- "გიორგი" : არის მნიშვნელობა რომელიც გვინდა შევინახოთ ცვლადში firstName.
- ; : სიმბოლო წერტილ-მძიმე გამოიყენება ინსტრუქციის დასასრულებლად.(ყველა ინსტრუქცია dart_ში უნდა დავასრულოთ ; _ ით)

ცვლადების შექმნა ასევე შეგვიძლია მონაცემის ტიპის მითითებით. ამ შემთხვევაში ჩვენ აღარ გვჭირდება var keyword_ის გამოყენება.

```dart
  String firstName = "გიორგი";
  int age = 27;
  
  print(firstName);
  print(age);
```

როგორც ხედავთ ამ შემთხვევაში ჩვენ გამოვიყენეთ მონაცემის ტიპები ცვლადების შესაქმნელად. პროგრამის გაშვების შედეგი იდენტურია <br /><br />
<img src="/screenshots/first_program.png" ><br />

რაში გვჭირდება ორი განსხვავებული მეთოდი ცვლადების შექმნისათვის? Dart_ი არის ეგრეთწოდებული Strongly Typed Language. ეს უბრალოდ იმას ნიშნავს, რომ პროგრამის გაშვებისას დარტმა უნდა იცოდეს ცვლადის მონაცემის ტიპი.
მაგრამ ჩვენ როდესაც ცვლადები var keyword_ის დახმარებით შევქმენით მონაცემის ტიპი არ მიგვითითებია. საქმე იმაშია რომ Dart_ს პროგრამის გაშვებისას შუაიძლია მონაცემის ტიპი ამოიკითხოს ცვლადის მნიშვნელობიდან. აქედან გამომდინარე ჩვენ შეგვიძლია გამოვიყენოთ ორივე მეთოდი და "ვენდოთ" დარტს, რომ ის სწორად გამოიცნობს ცვლადის მონაცემის ტიპს.

### მათემატიკური ოპერატორები
იმისათვის, რომ Dart_ში შევძლოთ მათემატიკური ოპერაციების შესრულება - ჩვენ გვჭირდება მათემატიკური ოპერატორები.
Dart_ში შევხვდებით შემდეგ მათემატიკურ ოპერატორებს:
1. მიმატება: '+' ოპერატორი გამოიყენება ორი რიცხვის შესაკრებად

```dart
    print(3 + 4); დაბეჭდავს 7_ს
```

2. გამოკლება: '-' ოპერატორი გამოიყენება ერთი რიცხვის მეორეზე გამოკლებისთვის

```dart
    print(7 - 4); დაბეჭდავს 3_ს
```

3. გამრავლება: '*' ოპერატორი გამოიყენება ერთი რიცხვის მეორეზე გასამრავლებლად


```dart
    print(3 * 4); დაბეჭდავს 12_ს
```

4. გაყოფა: '/' ოპერატორი გამოიყენება ერთი რიცხვის მეორეზე გასაყოფად

```dart
    print(12 / 4); დაბეჭდავს 3_ს
```

5. ნაშთი-modulus: '%' ოპერატორი გამოიყენება ერთი რიცხვის მეორეზე გაყოფისას არსებული ნაშთის გასაგებად.


```dart
    print(12 / 5); დაბეჭდავს 2_ს
```


### შედარების ოპერატორები
იმისათვის რომ ორი მნიშვნელობა ერთმანეთს შევადაროთ Dart_ში ვიყენებთ შედარების ოპერატორებს
Dart_ში შევხვდებით შემდეგ შედარების ოპერატორებს
1. ტოლია (==): ეს ოპერატორი ამოწმებს თუ კი ორი მნიშვნელობა ერთმანეთის ტოლია. თუ ტოლია აბრუნებს true, თუ არ არის ტოლი აბრუნებს false.

```dart
    var num1 = 3;
    var num2 = 3;

    print(num1 == num2)// დაბეჭდავს - true - რადგან 3 ტოლია 3_ის
    num1 = 4; // შევცვალეთ num1 იცვლადის მნიშვნელობა - გახდა 4
    print(num1 == num2)// დაბეჭდავს - false - რადგან 4 არ არის ტოლი 3_ის

```

2. არ არის ტოლი (!=): ეს ოპერატორი ამოწმებს თუ კი ერთი მნიშვნელობა არ არის ტოლი მეორესი. თუ არ არის ტოლი აბრუნებს true, თუ ტოლია აბრუნებს false (== ოპერატორის საპირისპირო)

```dart
    var num1 = 3;
    var num2 = 4;

    print(num1 != num2)// დაბეჭდავს - true - რადგან 3 არ არის ტოლი 4_ის
    num2 = 3; // შევცვალეთ num2 იცვლადის მნიშვნელობა - გახდა 3
    print(num1 != num2)// დაბეჭდავს - false - რადგან 3 ტოლია 3_ის

```
3. მეტია (>): ეს ოპერატორი ამოწმებს თუ კი მარცხნივ მდგომი მნიშვნელობა მეტია მარჯვნივ მდგომ მნიშვნელობაზე.
თუ მეტია აბრუნებს true, თუ არ არის მეტი აბურნებს false.

```dart

    var num1 = 10;
    var num2 = 5;

    print(num1 > num2)// დაბეჭდავს - true - რადგან 10 მეტია 5_ზე
    num2 = 10; // შევცვალეთ num2 იცვლადის მნიშვნელობა - გახდა 10
    print(num1 > num2)// დაბეჭდავს - false - რადგან 10 არ არის მეტი 10_ზე
    num2 = 20; // შევცვალეთ num2 იცვლადის მნიშვნელობა - გახდა 20
    print(num1 > num2)// დაბეჭდავს - false - რადგან 10 არ არის მეტი 20_ზე

```

4. მეტია ან ტოლია (>=): ეს ოპერატორი ამოწმებს თუ კი მარცხნივ მდგომი მნიშვნელობა მეტია ან ტოლია მარჯვნივ მდგომ მნიშვნელობაზე.
თუ მეტია ან ტოლია აბრუნებს true, თუ არ არის მეტი ან ტოლი აბურნებს false.

```dart

    var num1 = 10;
    var num2 = 5;

    print(num1 >= num2)// დაბეჭდავს - true - რადგან 10 მეტია 5_ზე
    num2 = 10; // შევცვალეთ num2 იცვლადის მნიშვნელობა - გახდა 10
    print(num1 >= num2)// დაბეჭდავს - true - რადგან 10 არ არის მეტი მაგრამ ტოლია 10_ის
    num2 = 20; // შევცვალეთ num2 იცვლადის მნიშვნელობა - გახდა 20
    print(num1 >= num2)// დაბეჭდავს - false - რადგან 10 არ არის არც მეტი და არც ტოლი 20_ის

```

5. ნაკლებია (<): ეს ოპერატორი ამოწმებს თუ კი მარცხნივ მდგომი მნიშვნელობა ნაკლებია მარჯვნივ მდგომ მნიშვნელობაზე.
თუ ნაკლებია აბრუნებს true, თუ არ არის ნაკლები აბურნებს false.


```dart

    var num1 = 10;
    var num2 = 5;

    print(num1 < num2)// დაბეჭდავს - false - რადგან 10 არ არის ნაკლები 5_ზე
    num2 = 10; // შევცვალეთ num2 იცვლადის მნიშვნელობა - გახდა 10
    print(num1 < num2)// დაბეჭდავს - false - რადგან 10 არ არის ნაკლები 10_ზე
    num2 = 20; // შევცვალეთ num2 იცვლადის მნიშვნელობა - გახდა 20
    print(num1 < num2)// დაბეჭდავს - true - რადგან 10 ნაკლებია 20_ზე

```

6. მეტია ან ტოლია (<=): ეს ოპერატორი ამოწმებს თუ კი მარცხნივ მდგომი მნიშვნელობა ნაკლებია ან ტოლია მარჯვნივ მდგომ მნიშვნელობაზე.
თუ მეტია ან ნაკლებია აბრუნებს true, თუ არ არის ნაკლები ან ტოლი აბურნებს false.

```dart

    var num1 = 10;
    var num2 = 5;

    print(num1 <= num2)// დაბეჭდავს - false - რადგან 10 არ არის არც ნაკლები არც ტოლი 5_ის
    num2 = 10; // შევცვალეთ num2 იცვლადის მნიშვნელობა - გახდა 10
    print(num1 <= num2)// დაბეჭდავს - true - რადგან 10 არ არის ნაკლები მაგრამ ტოლია 10_ის
    num2 = 20; // შევცვალეთ num2 იცვლადის მნიშვნელობა - გახდა 20
    print(num1 <= num2)// დაბეჭდავს - true - რადგან 10 ნაკლებია 20_ზე

```

### როგორ მივიღოთ მომხმარებლისგან ინფორმაცია?
ხშირად პროგრამაში გვჭირდება მომხმარებლისაგან მივიღოთ რაიმე ინფორმაცია. ამისათვის Dart_ი გვაწვდის 'stdin'(standard input) ბიბლიოთეკას, რომლის დახმარებით შეგვიძლია წავიკითხოთ მომხმარებლის მიერ შეყვანილი ტექსტი კონსოლში (იგივე ტერმინალი ან CMD).

```dart
import 'dart:io';

void main() {
    print('Please enter your name: ');
    String? name = stdin.readLineSync();
    print('Hello, $name!');
}
```

!!! ეს კოდის ფრაგმენტი არ იმუშავებს DartPad_ში.

კოდის პირველ ხაზზე გვხვდება Dart_ის ჯერჯერობით ჩვენთვის უცნობი სინტაქსი - import 'dart:io'; import keyword_ი პროგრამას მიუთითებს, რომ გვჭირდება გამოვიყენოთ კოდი რომელიც სხვა ფაილში ან სხვა ბიბლიოთეკაშია. 'dart:io' არის უნიკალური გზა რომელიც პროგრამას ეუბნება ადგილმდებარეობას თუ საიდან უნდა მოიტანოს ეს ფაილი თუ ბიბლიოთეკა. შესაბამისად ამ ინსტრუქციის შესრულების შემდეგ ჩვენ შეგვეძლება გამოვიყენოთ ფუნქციონალი რომელიც dart:io ბიბლიოთეკაშია აღწერილი.
main ფუნქციაში პირველი ინსტრუქცია კონსოლში მომხმარებელს სთხოვს შეიყვანოს სახელი.
შემდეგ ინსტრუქციაში ჩვენ ვქმნით String? ცვლადს სახელად name და ვანიჭებთ მნიშვნელობას, რომელსაც readLineSync() ფუნქცია დააბრუნებს. stdin არის ობიექტი რომელსაც 'აქვს' ფუნქცია readLineSync(). readLineSync ფუნქცია თავის მხრივ პასუხისმგებელია კონსოლში მომხმარებლის მიერ შეყვანილი ინფორმაციის წაკითხვაზე.

!!! stdin.readLineSync() ფუნქციამ შეიძლება ვერ მოახერხოს ინფორმაციის წაკითხვა კონსოლიდან(სხვადასხვა მიზეზის გამო) და დააბრუნოს null (null _ზე მოგვიანებით ვისაუბრებთ. ახლა უბრალოდ წარმოიდგინეთ რომ null ნიშნავს არაფერს, მნიშვნელობის არ არსებობას). ამიტომ ცვლადის შექმნისას მონაცემის ტიპ String_ს მივუწერეთ ? რაც მიუთითებს იმაზე რომ ამ ცვლადს შეუძლია შეინახოს როგორც String მნიშვნელობა ასევე null.
შემდეგ ხაზზე კი ჩვენ უბრალოდ ვბეჭდავთ მისალმებას და მომხმარებლის სახელს.

### როგორ მივიღოთ გადაწყვეტილება - if else
Dart_ში 'if'/'else' სინტაქსი საშვალებას გვაძლევს მივიღოთ გადაწყვეტილება და შევასრულოთ განსხვავებული კოდის ფრაგმენტი რაიმე პირობის მიხედვით.
ზოგადი 'if'/'else' სინტაქსი Dart_ში ასე გამოიყურება:

```dart
if (პირობა) {
  //კოდის ფრაგმენტი რომელიც შესრულდება თუ კი პირობა დააბრუნებს true მნიშვნელობას
} else {
  //კოდის ფრაგმენტი რომელიც შესრულდება თუ კი პირობა დააბრუნებს false მნიშვნელობას
}
```

"პირობა"_მ აუცილებლად უნდა დააბრუნოს true ან false. ნებისმიერი სხვა მნიშვნელობა არის სინტაქსური შეცდომა.

აღსანიშნავია, რომ 'else' ინსტრუქცია არ არის სავალდებულო და შეგვიძლია გამოვტოვოთ.

ქვემოთ მოცემული პროგრამა ამოწმებს რაიმე რიცხვი არის თუ არა ლუწი.

```dart
int num1 = 23;

if (num1 % 2 == 0) { //თუ num1 ის 2 ზე გაყოფისას ნაშთი არის 0
  print("$num1 არის ლუწი");
} else {
  print("$num1 არის კენტი");
}
```


### როგორ გავიმეოროთ ერთი და იგივე კოდის ფრაგმენტი - loops

### კლასები და ობიექტები

### სიები