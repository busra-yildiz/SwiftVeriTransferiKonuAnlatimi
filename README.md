# SwiftVeriTransferiKonuAnlatimi
Swift (Swift for iOS) programlama dili ile veri transferi, genellikle iOS uygulamaları içinde farklı ekranlar veya görünümler arasında bilgi veya veri iletişimi sağlamak için kullanılır. Bu işlem için iki yaygın yöntem vardır: "Segue" kullanarak ve "Delegate" desenini kullanarak veri aktarımı. İşte her iki yöntemi de açıklamak için temel adımlar:

Yöntem 1: Segue Kullanarak Veri Aktarımı

İlk Ekranı Hazırlama:
İlk ekran (kaynak ekran) içinde veriyi göndermek istediğiniz veriyi bulundurun. Bu veriyi bir değişkene veya özelliklere atayın. Örneğin, bir metin girişi kutusu içindeki metni almak için bir değişken kullanabilirsiniz.
Segue'i Hazırlama:
Interface Builder'ı kullanarak veya programatik olarak, ekranlar arası geçişi tanımlayan bir "segue" oluşturun. Bu geçiş, kullanıcının bir düğmeye tıkladığında veya belirli bir olay gerçekleştiğinde tetiklenebilir.
Segue'ye Hazırlık:
Segue'yi başlatmadan önce, veriyi hedef ekrana aktarabilmek için prepare(for:sender:) yöntemini kullanarak hedef ekranı ayarlayın. Bu yöntemi kullanarak verileri hedef ekranın özelliklerine aktarabilirsiniz.
Hedef Ekranı Ayarlama:
prepare(for:sender:) yöntemi içinde hedef ekranı, verileri alacak şekilde ayarlayın. Örneğin, verileri hedef ekranın özelliklerine atayabilirsiniz.
Segue'yi Tetikleme:
Segue'yi başlatmak için belirli bir olayı kullanın, genellikle bir düğmeye tıklama veya belirli bir işlem gerçekleştikten sonra.
Yöntem 2: Delegate Deseni Kullanarak Veri Aktarımı

Delegate deseni, bir ekranın (kaynak ekran) diğer bir ekrana (hedef ekran) veri aktarmasına olanak tanır. Temel adımlar şunlardır:

Delegate Protokolünü Tanımlama:
İlk adım, veri aktarımı için bir delegate protokolünü tanımlamaktır. Bu protokol, hedef ekranın uygulaması tarafından uygulanmalıdır.
Delegate Değişkenini Tanımlama:
Kaynak ekran, hedef ekranın delegate'ine erişmek için bir değişken tanımlar.
Veriyi Delegate Aracılığıyla Aktarma:
Kaynak ekran, veriyi hedef ekranın delegate'ine gönderir. Hedef ekran bu veriyi alır ve işler.
Delegate'i Ayarlama:
Kaynak ekran, kendisini hedef ekranın delegate'i olarak ayarlar.
Bu yöntem, belirli bir olayın gerçekleştiğinde veri aktarımını tetiklemek için kullanışlıdır. Örneğin, bir kullanıcı bir düğmeye tıkladığında veya belirli bir işlemi tamamladığında veri aktarımı gerçekleşebilir.

Swift ile veri transferi bu iki yöntem aracılığıyla yapılabilir. Hangi yöntemin kullanılacağı, uygulamanızın ihtiyaçlarına ve tasarımına bağlıdır.
