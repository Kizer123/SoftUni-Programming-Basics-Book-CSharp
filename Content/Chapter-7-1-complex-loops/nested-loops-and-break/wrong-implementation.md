#### Грешна имплементация

Ето едно **грешно решение**, което изглежда правилно на пръв поглед:

![](/assets/chapter-7-images/00.Nested-and-break-desired-result-02.png)

Ако оставим програмата ни по този начин, резултатът ни ще е следният:

![](/assets/chapter-7-images/00.Nested-and-break-undesired-result-01.png)

Защо се получава така? Както виждаме, в резултата **липсва "1 1"**. Когато програмата стига до там, че **`i = 1`** и **`j = 1`**, тя влиза в **`if`** проверката и изпълнява **`break`** операцията. По този начин се **излиза от вътрешния цикъл**, но след това продължава изпълнението на външния. **`i`** нараства, програмата влиза във вътрешния цикъл и принтира резултата.

<table><tr><td><img src="/assets/alert-icon.png" style="max-width:50px" /></td>
<td>Когато във <b>вложен цикъл</b> използваме оператора <b><code>break</code></b>, той прекъсва изпълнението <b>само</b> на вътрешния цикъл.</td>
</tr></table>