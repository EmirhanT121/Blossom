# Blossom
Blossom algoritması, arama işleme işi için uygun değildir. Bu yüzden sadece Boyer-Moore Algoritması için kod yazdım.

Blossom algoritması, kombinatorik optimizasyon problemleri için bir çözümleme yöntemidir. Kombinatorik optimizasyon problemleri, birçok farklı seçenek arasından en iyi olanını bulmak için matematiksel modelleme ve optimizasyon tekniklerini kullanarak çözülen problemlerdir.

Blossom algoritması, özellikle en az maliyetli eşleştirme (minimum cost matching) sorununu çözmek için kullanılır. En az maliyetli eşleştirme sorunu ise iki farklı küme arasında yapılan bir eşleştirme işlemidir. Örneğin, birinci kümede bulunan elemanlar ile ikinci kümede bulunan elemanlar arasında bir eşleştirme yapmak istenildiğinde, her bir eşleştirme için bir maliyet belirtilir. Bu maliyetlerin toplamı en az olacak şekilde bir eşleştirme yapmak istendiğinde en az maliyetli eşleştirme sorunu ortaya çıkar.

Blossom algoritması, bu sorunu çözmek için bir graf teorisi algoritmasıdır. İlk olarak, graf teorisinde bir kavram olan "çiçek"leri kullanır. Bu kavram, graf içinde belirli bir şekilde birleştirilmiş düğümler kümesine verilen isimdir.

Algoritma, başlangıçta her bir elemanı bir çiçek olarak ele alır. Daha sonra, graf içinde belirli bir şekilde eşleştirmeler yaparak, çiçeklerin birleştirilmesiyle yeni çiçekler oluşturur. Bu işlem, en az maliyetli eşleştirme sorununu çözmeye kadar devam eder.

Blossom algoritması, polinom zamanlı bir algoritma olduğu için, büyük boyutlu problemleri çözmek için oldukça uygundur. Ayrıca, en az maliyetli eşleştirme sorununun yanı sıra, diğer kombinatorik optimizasyon problemlerinin de çözümünde kullanılabilir.

En iyi durumda, yani eşleştirme hali zaten tam ve algoritma herhangi bir işlem yapmadan çıkarsa, algoritmanın çalışma zamanı O(n^3) olacaktır.

Ortalama durumda, algoritmanın çalışma zamanı O(n^3) 'e yakın olabilir. Bu durumda, bir dizi rastgele eşleştirme yaparak ve bunları güncelleyerek, en az maliyetli eşleştirme probleminin çözümüne yaklaşılabilmektedir.

En kötü durum, tamamen eşleştirilmiş olmayan bir grafa sahip olmaktır. Bu durumda, algoritmanın her adımında bir yeni çiçek yaratılacak ve tüm çiçekler yeniden işlenecektir. Bu nedenle, her adımda O(n^2) çiçek oluşur ve bu adım O(n^3) zaman alır. Toplam zaman, O(n^4) olacaktır.
