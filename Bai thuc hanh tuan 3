import 'dart:convert';
import 'dart:io';
import 'dart:math';

void e1(String name){ // Write a program in Dart to print your own name using function.
  print("Your name is $name");
}
void e2(int l, int r){ // Write a program in Dart to print even numbers between intervals using function
  assert(l <= r);
  if(l % 2 == 1){
    ++l;
  }
  if(r % 2 == 1){
    --r;
  }
  for(int i = l; i <= r; i+=2){
    stdout.write('$i ');
  }
}
String e3_passwordGenerator(int passwordLength) {
  if(passwordLength < 1) return "";
  final random = Random.secure();
  List<int> intList = List.generate(passwordLength, (_) => random.nextInt(255));
  List charList = base64UrlEncode(intList).split('').toList();
  charList.shuffle();
  return charList.join('');
}
double area_of_circle(double r){
  return r * r * pi;
}
void e4_find_area_of_circle(){
  stdout.write("Enter radius: ");
  double radius = double.parse(stdin.readLineSync()!);
  print("Area = ${area_of_circle(radius)}");
}
double find_squared_angle(double a, double c){
  return sqrt(c * c - (a * a));
}
double find_hypotenuse(double a, double b){
  return sqrt((a * a) + (b * b));
}
void e5_Pytagon(){
  print("Enter your chosen: ");
  print("1. Find hypotenuse");
  print("2. Find squared angle");
  int chosen = int.parse(stdin.readLineSync()!);
  assert(chosen == 1 || chosen == 2);
  if (chosen == 1){
    print("Enter a, b: ");
    double a = double.parse(stdin.readLineSync()!);
    double b = double.parse(stdin.readLineSync()!);
    print("Hypotenuse = ${find_hypotenuse(a, b)}");
  }
  else {
    print("Enter a, c: ");
    double a = double.parse(stdin.readLineSync()!);
    double c = double.parse(stdin.readLineSync()!);
    print("Squared angle = ${find_squared_angle(a, c)}");
  }
}
String reverse(String s){
  final str = s.runes.toList();  
  return String.fromCharCodes(str.reversed);
} 
void e6_reverse(){
  stdout.write("Enter your string: ");
  String s = stdin.readLineSync()!;
  print("Reversed string = ${reverse(s)}");
}

void e7(){
  stdout.write("Enter base: ");
  double base = double.parse(stdin.readLineSync()!);
  stdout.write("Enter exponent: ");
  double exponent = double.parse(stdin.readLineSync()!);
  print("$base ^ $exponent = ${pow(base,exponent)}");
}
