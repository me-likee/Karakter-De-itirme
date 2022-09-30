# Karakter-De-itirme
// Verilen string ifade içerisindeki ilk ve son karakterin yerini değiştirip tekrar ekrana yazdıran console uygulamasını yazınız.

// Örnek: Input: Merhaba Hello Algoritma x

//        Output: aerhabM oellH algoritmA x
   var metin = Console.ReadLine().Split(' ');
    foreach (var i in metin)
    {
        int boyut = i.Length;
        string ters = i;
        string basharf = ters[0].ToString();
        string sonharf = ters[i.Length - 1].ToString();
        ters = ters.Remove(0, 1);//Baş harfi Sildik
        ters = ters.Remove(boyut-2,1);//Son Harfi Sildik
        ters = sonharf+ters + basharf;
        Console.Write(ters + " ");
    }
