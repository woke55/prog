Primjer1: Napisati klasu Trougao. Napisati kratak test program.
• //Datoteka: Trougao.h
• #ifndef TROUGAO_H
• #define TROUGAO_H
• #include<math.h>
• #include<iostream>
• using namespace std;
• class Trougao
• {
• private:
• /* PODACI - CLANOVI */
• double a;
• double b;
• double c;
• public:
• /* METODE */
• /* Konstruktor */
• Trougao() {a=3; b=4; c=5;} 
  
 //Datoteka: Trougao.cpp
• #include "Trougao.h"
• double Trougao::getO() const
• {
• return a+b+c;
• }
• double Trougao::getP() const
• {
• double s=(a+b+c)/2;
• return sqrt(s*(s-a)*(s-b)*(s-c));
• }
• //DAtoteta: test.cpp
• int main()
• {
• Trougao t;
• cout<<"Stranica a: "<<t.getA()<<endl;
• cout<<"Stranica b: "<<t.getB()<<endl;
• cout<<"Stranica c: "<<t.getC()<<endl;
• cout<<"Obim: "<<t.getO()<<endl;
• cout<<"Povrsina: "<<t.getP()<<endl;
• return 0;
• } 
  
  Primjer2: Napisati klasu Kvadrat. Napisati kratak test program. 
  •//Datoteka: Kvadrat.h
•#ifndef KVADRAT_H
•#define KVADRAT_H
•#include<math.h>
•#include<iostream>
•using namespace std;
•class Kvadrat
•{
• private:
•/* PODACI - CLANOVI */
• double a;
• public:
•/* METODE */
• /* Konstruktor */
• Kvadrat() {a=5;}
• /* SET-metode */
• void setA(double aa) { a = aa; }
• /* GET-metode */
• double getA() const { return a; }
• /* OSTALE-metode */
• double getO() const;
• double getP() const;
•};
•#endif // KVADRAT_H 
  
  •//Datoteka: Kvadrat.cpp
•#include "Kvadrat.h"
•double Kvadrat::getO() const
•{
• return 4*a;
•}
•double Kvadrat::getP() const
•{
• return pow(a, 2);
•}
•//Datoteta: test.cpp
•int main()
•{
• Kvadrat k;
• cout<<"Stranica a: "<<k.getA()<<endl;
• cout<<"Obim: "<<k.getO()<<endl;
• cout<<"Povrsina: "<<k.getP()<<endl;
• return 0;
  
  1. Kreirati klasu KUTIJA.
class Kutija
{
double duzina;
double sirina;
double visina;
void pakovanje ();
};

 2. Kreirati klasu PAS.
class Pas
{
int starost;
int tezina;
double sirina;
string boja;
void lajati ();
};
  
 Primjer: klasa koja sadrzi konstruktor bez parametara, konstruktor sa parametrima
i konstruktor kopije. 
  #ifndef MOJAKLASA_H
#define MOJAKLASA_H
class MojaKlasa
{
 private:
int x;
public:
 MojaKlasa() {x=5; }
MojaKlasa (int xx) {x=xx;}
MojaKlasa (const MojaKlasa &m) {x=m.x; }
 void setX(int xx) { x = xx; }
int getX () const { return x; }
};
#endif // MOJAKLASA_H 
•} 
