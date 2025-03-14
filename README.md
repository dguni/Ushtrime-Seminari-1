# Ushtrime-Seminari-1
//Ush1
Console.WriteLine("Emri:");
string emri = Console.ReadLine();
Console.WriteLine("Mbiemri: ");
string mbiemri = Console.ReadLine();
Console.WriteLine("Mosha: ");
string mosha = Console.ReadLine();
Console.WriteLine("Profesioni: ");
string profesioni = Console.ReadLine();
Console.WriteLine($"Emri: {emri}, Mbiemri: {mbiemri}, Mosha: {mosha}, Profesioni: {profesioni}");

//Ush2
Console.WriteLine("Shkruani numrin e pare: ");
int nr1 = Convert.ToInt32(Console.ReadLine());
Console.WriteLine("Shkruani numri e dyte: ");
int nr2 = Convert.ToInt32(Console.ReadLine());
if (nr1 > nr2)
{
    int mbetja = nr1 % nr2;
    Console.WriteLine($"Mbetja e {nr1} dhe {nr2} eshte: {mbetja}");
}
else
{
    Console.WriteLine("Gabim. Numri 1 duhet te jete me i madh se numri 2");
}
//Ush3
int[] numrat = new int[5];
int shuma = 0;

Console.WriteLine("Shkruani 5 numra:");

for (int i = 0; i < 5; i++)
{
    Console.Write($"Numri {i + 1}: ");
    numrat[i] = Convert.ToInt32(Console.ReadLine());
    shuma += numrat[i];
}

double mesatarja = (double)shuma / 5;

Console.WriteLine($"Shuma: {shuma}");
Console.WriteLine($"Mesatarja: {mesatarja}");

//Ush4
int a = -10 + 7 * 5;
int b = (25 + 4) % 9;
int c = 10 + 3 - 3 * 4 / 9;
int d = 1 + 23 / 3 * 2 - 7 % 3;
Console.WriteLine($"-10 + 7 * 5={a}");
Console.WriteLine($"(25 + 4) % 9={b}");
Console.WriteLine($"10 + 3 - 3 * 4 / 9={c}");
Console.WriteLine($"1 + 23 / 3 * 2 - 7 % 3={d}");

//Ush5
Console.WriteLine("Shkruani numrin e pare: ");
int nr1 = Convert.ToInt32(Console.ReadLine());
Console.WriteLine("Shkruani numrin e dyte: ");
int nr2 = Convert.ToInt32(Console.ReadLine());
if (nr1 > nr2)
{
    int mbetja = nr1 % nr2;
    Console.WriteLine($"Mbetja e {nr1} dhe {nr2} eshte: {mbetja}");
}
else
{
    Console.WriteLine("Gabim.Numri 1 duhet te jete me i madh se numri 2");
}

//Ush6
Console.WriteLine("Shkruani gjatesine e drejtkendeshit: ");
double gjatesia = Convert.ToDouble(Console.ReadLine());
Console.WriteLine("Shkruani gjeresine e drejtkendeshit: ");
double gjeresia = Convert.ToDouble(Console.ReadLine());
double perimetri = 2 * (gjatesia + gjeresia);
double siperfaqja = gjatesia * gjeresia;
Console.WriteLine($"Perimetri i drejtkendeshit eshte: {perimetri}");
Console.WriteLine($"Siperfaqja e drejtkendeshit eshte: {siperfaqja}");

//Ush7
Console.WriteLine("Jepni numrin e pare: ");
int nr1 = Convert.ToInt32(Console.ReadLine());
Console.WriteLine("Jepni numrin e dyte: ");
int nr2 = Convert.ToInt32(Console.ReadLine());
nr1 = nr1 + nr2;
nr2 = nr1 - nr2;
nr1 = nr1 - nr2;
Console.WriteLine($"Pas shkembimit: Numri i pare={nr1}, Numri i dyte={nr2}");

//Ush8
List<string> titujt = new List<string>();
List<string> autoret = new List<string>();
List<double> cmimet = new List<double>();

for (int i = 0; i < 3; i++)
{
Console.WriteLine($"Libri {i + 1}:");
Console.Write("Titulli: ");
titujt.Add(Console.ReadLine());

Console.Write("Autori: ");
autoret.Add(Console.ReadLine());

Console.Write("Cmimi: ");
cmimet.Add(double.Parse(Console.ReadLine()));

Console.WriteLine();
}

Console.WriteLine("Librat e futur:");
for (int i = 0; i < titujt.Count; i++)
{
    Console.WriteLine($"Titulli: {titujt[i]}, Autori: {autoret[i]}, Çmimi: {cmimet[i]} EUR");

//Ush9
    Console.WriteLine("Zgjidhni monedhen e konvertimit:");
    Console.WriteLine("1. Nga EUR ne USD");
    Console.WriteLine("2. Nga USD ne EUR");
    Console.Write("Zgjedhja: ");
    int zgjedhja = int.Parse(Console.ReadLine());

    Console.Write("Shuma per konvertim: ");
    double shuma = double.Parse(Console.ReadLine());

    double kursiEurNeUsd = 1.09;
    double kursiUsdNeEur = 0.92;

    double rezultati = 0;

    if (zgjedhja == 1)
    {
        rezultati = shuma * kursiEurNeUsd;
        Console.WriteLine($"{shuma} EUR = {rezultati:F2} USD");
    }
    else if (zgjedhja == 2)
    {
        rezultati = shuma * kursiUsdNeEur;
        Console.WriteLine($"{shuma} USD = {rezultati:F2} EUR");
    }
    else
    {
        Console.WriteLine("Zgjedhje e pavlefshme!");

//Ush10
Console.WriteLine("Jepni nje numer: ");
int nr = Convert.ToInt32(Console.ReadLine());
for(int i = 0; i <= 10; i++)
{
    int rezultati = nr * i;
    Console.WriteLine($"{nr}*{i}={rezultati}");
}
