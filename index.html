import { useState, useEffect, useRef } from "react";

// ─── MƏTNLƏRİN TƏRKİBİ ───────────────────────────────────────────────────────
const texts = {
  badii: {
    id: "badii",
    title: "Bədii mətn",
    source: "(Aytən Yadigarlı \u201cYuxunun sehri\u201d kitabından)",
    content: [
      { type: "p", text: "Geniş zalın yuxarı başında ", parts: [{ t: "azəmətli", bold: true, underline: true }, { t: " bir şah taxtı qoyulmuşdu. Cavanşir şah taxtında əyləşmiş, ətrafındakılar da böyük səbirsizliklə onun danışmasını gözləyirdilər." }] },
      { type: "p", text: "Şah taxtından qalxdı və gur səslə danışmağa başladı:" },
      { type: "dialog", text: "— Bu döyüşdə mütləq qalib gəlməliyik! Əsirlikdə olan bütün həmvətənlərimiz azad edilməlidir! Torpaqlarımızdan düşməni qovmalıyıq!" },
      { type: "p", text: "Vəzir dilləndı:" },
      { type: "dialog", text: "— Şah sağ olsun, müharibəni davam etdirsək, çox itkimiz olacaq. Düşünürəm ki, torpaqlarımızdan bir qarış versək, heç nə olmaz. Əvəzində qalan əhalimiz sağ qalar. Heç olmasa, onları xilas edə bilərik." },
      { type: "p", text: "Şah qəzəbləndi. Bunu onun çatılmış qaşlarından da, zəhmli səsindən də hiss etmək olurdu:" },
      { type: "dialog", text: "— Nə danışırsan, vəzir? Bu nə sözdür, deyirsən? İnsan Vətəni qanı, canı bahasına olsa da, qorumalıdır. Bir qarış torpaq nə deməkdir? Heç bir misqal da Vətən torpağından pay ola bilməz! Sənin əlini və ya ayağını kəssək, bir gözünü kor etsək, necə olar? Onlar sənin varlığının bir parçası olduğu kimi torpaq da Vətənin canı, qanı, parçasıdır! Mən Vətənimin bir parçası üçün bütün varlığımdan keçməyə hazıram!" },
      { type: "p", text: "Vəzirlərdən biri dilləndı:" },
      { type: "dialog", text: "— Şah sağ olsun!" },
      { type: "dialog", text: "— Söhbət bitdi! Bu məsələ ilə bağlı etiraz eşitmək istəmirəm! Döyüş olacaq!" },
    ]
  },
  informativ: {
    id: "informativ",
    title: "Gələrsən-Görərsən qalası – İnformativ Mətn",
    source: "",
    content: [
      { type: "num", n: "1.", text: "Gələrsən-Görərsən qalası Şəkinin Kiş kəndinin şimal-şərqində, Qaratəpə dağının üzərində yerləşir. Qaratəpə dağının arxasında isə yüksək dağlar sıralanır." },
      { type: "p", text: "Qalanın belə bir yerdə salınmasının əsas məqsədi odur ki, sıldırım olduğuna görə qalaya öndən, arxadan və çay tərəfdən hücum etmək mümkün olmasın. Qala ilə Kiş kəndi arasındakı ərazi Qala düzü də adlanır." },
      { type: "p", text: "Gələrsən-Görərsən qalası sındırılmış çay daşlarından inşa edilmişdir. Şəki şəhərinin özü qala divarları ilə əhatə olunmadığı üçün düşmən hücum edən zaman əhali Gələrsən-Görərsən qalasına sığınırdı." },
      { type: "num", n: "2.", text: "Qalanı seyr etdikcə qandan-qadadan, amansız savaş və qovğalardan xəbər verən ötən çağlar gözümüz qarşısında canlanır." },
      { type: "num", n: "3.", text: "Adama elə gəlir ki, bu qalanın möhkəm divarları, uca bürclər, ", parts: [{ t: "nəhəng", bold: true, underline: true }, { t: " qüllələri öz əzmi ilə yenilmək, əyilmək bilməyən igidlər, ana yurdun keşiyində dayanıb. Qalada aparılan açıq savaşda onunla bacara bilməyəcəyini dərk edən Şəki vilayətinin hakimi Hacı Çələbi xan qalaya sığınaraq müqavimət göstərməyi qərara alıb. Nadir şah Hacı Çələbi xana məktub yazaraq qalanın təslim edilməsini tələb etmiş, əks halda torpağını yerə-yeksan edəcəyini, qaladakıların hamısını qılıncdan keçirəcəyini bəyan edib. Qalanın igid müdafiəçiləri isə ona açıq cavab verərək Gələrsən, görərsən — deyiblər." }] },
      { type: "num", n: "4.", text: "Azərbaycanın tanınmış şairləri çoxdur. Bir çox yazıçılar öz əsərlərində Gələrsən-Görərsən qalasından bəhs etmişlər." },
    ]
  }
};

// ─── SUALLAR ─────────────────────────────────────────────────────────────────
const questions = [
  // Bədii mətn sualları 1-15
  { id:1, textId:"badii", subject:"Azərbaycan dili", text:"Hansı atalar sözü mətnin ideyasını özündə əks etdirir?", options:["Dünyada vətəndən əziz nə var?","Doğma yurd şirin olar.","Bu dünyada şirin şey, bir anadır, bir vətən.","El gücü, sel gücü."], answer:"C" },
  { id:2, textId:"badii", subject:"Azərbaycan dili", text:"Hansı epizodda Cavanşir şahın qəzəblənməsi nəzərə çarpır?", options:["Şahın taxtında əyləşməsi","Şahın qalib olmaq istəyi","Döyüş əmrinin verilməsi","Vəzirin şahla söhbəti"], answer:"D" },
  { id:3, textId:"badii", subject:"Azərbaycan dili", text:"Şah nəyə görə döyüşün olmasını israrla istəyirdi?\n1. Müharibəni çox sevirdi.\n2. Düşmənləri torpağından qovmaq istəyirdi.\n3. Qan tökmək, qisas almaq niyyəti var idi.\n4. Əsir düşmüş həmvətənlərini xilas etmək istəyirdi.", options:["1, 2","1, 4","2, 4","1, 3"], answer:"B" },
  { id:4, textId:"badii", subject:"Azərbaycan dili", text:"Cavanşir şah obrazı ilə bağlı səhv fikir hansıdır?", options:["Vətənini canından çox sevir.","Müharibəni qalib gəlmək istəyir.","Əhaliyə zülm edir.","Qorxmazdır."], answer:"C" },
  { id:5, textId:"badii", subject:"Azərbaycan dili", text:"Vəzirin müharibənin dayanmasını istəməsinin səbəbi ola bilər:", options:["Çünki itkinin çox olacağını düşünürdü.","Çünki döyüşə bilmirdi.","Çünki düşmən məğlubiyyətini boynuna almışdı.","Çünki artıq qələbə qazanılmışdı."], answer:"A" },
  { id:6, textId:"badii", subject:"Azərbaycan dili", text:"Mətnin mövzusunu müəyyənləşdirin.", options:["Dostluq","Yurd həsrəti","Xeyirxahlıq","Vətənə sevgi"], answer:"D" },
  { id:7, textId:"badii", subject:"Azərbaycan dili", text:"Mətnə əsasən klasteri tamamlayacaq fikri seçin.\n(Vəzir → Döyüşün davam etməyini istəmir → ?)", options:["Çox cəsurdur.","Vətən torpağından bir qarış düşmənə vermək istəyir.","Zəfər çalmaq üçün vuruşur.","Vətən onun üçün müqəddəsdir."], answer:"D" },
  { id:8, textId:"badii", subject:"Azərbaycan dili", text:"Mətnin məzmununa uyğun gələn başlıq hansıdır?", options:["Cavanşir şahın zülmkarlığı","Əziz Vətən","Hiyləgar vəzir və şah","İtirilmiş qələbə"], answer:"B" },
  { id:9, textId:"badii", subject:"Azərbaycan dili", text:"Hansı fikir Cavanşir şahın xarakterinin açılmasına kömək edir?", options:["Onun çox vahiməli görünüşü və qəzəbli baxışları var idi.","İnsan Vətənini canı, qanı bahasına da olsa, qorumalıdır.","O, geniş zalın yuxarı başında, öz taxtında əyləşmişdi.","Şah taxtından qalxar-qalxmaz sözə başladı."], answer:"B" },
  { id:10, textId:"badii", subject:"Azərbaycan dili", text:"Mətndə qırmızı hərflərlə verilmiş sözü (azəmətli) əvəz edə bilməz:", options:["qiymətli","dəbdəbəli","təmtəraqlı","möhtəşəm"], answer:"B" },
  { id:11, textId:"badii", subject:"Azərbaycan dili", text:"Cavanşir şah obrazına aid olmayan xüsusiyyət hansıdır?", options:["vətənpərvər","mərd","cəsur","etibarsız"], answer:"D" },
  { id:12, textId:"badii", subject:"Azərbaycan dili", text:"Verilmiş cümləni məntiqi cəhətdən tamamlayan fikir hansıdır?\n\n«Vəzirin dedikləri ...»", options:["şahı qəzəbləndirdi.","şahın xoşuna gəldi.","ətrafdakıları sevindirdi.","düşmənlərin işinə yaradı."], answer:"A" },
  { id:13, textId:"badii", subject:"Azərbaycan dili", text:"Mətndə hansı sualın cavabını tapmaq olmaz?", options:["Cavanşir şahın istəyi nə idi?","Vəzir sağ qalan əhalini xilas etmək üçün hansı yolu təklif etdi?","Döyüşdə kimin qoşunu qalib gəldi?","Şahın qəzəblənməyinə səbəb nə idi?"], answer:"C" },
  { id:14, textId:"badii", subject:"Azərbaycan dili", text:"Mətnlə bağlı verilmiş fikirlərdən hansı düzgün deyil?", options:["Cavanşir şahın həyatından bəhs olunur.","Mətndə heç bir fakta rast gəlinmir.","Dialoq şah və vəzir arasındadır.","Şah sarayı təsvir edilir."], answer:"B" },
  { id:15, textId:"badii", subject:"Azərbaycan dili", text:"Cavanşir şahın fikrincə, ....", options:["qələbə qazanmaq mümkün olmayacaq.","torpaq Vətənin bir parçasıdır.","əsirləri xilas etməyə dəyməz.","düşmənə torpaqları bağışlamaq olar."], answer:"B" },
  { id:16, textId:"badii", subject:"Azərbaycan dili", text:"Nömrələnmiş cümlələrdən hansı mətnə uyğun gəlmir?", options:["1","2","3","4"], answer:"B" },
  // İnformativ mətn sualları 17-30
  { id:17, textId:"informativ", subject:"Azərbaycan dili", text:"Qalada aparılan araşdırmalara əsasən aşkar olunub:", options:["şah və ailəsinə məxsus geyimlər","saxsı qab qırıqları","döyüşçülərin dəbilqə və qılıncları","su içmək üçün qablar"], answer:"B" },
  { id:18, textId:"informativ", subject:"Azərbaycan dili", text:"Qalanı qoruyan, məğrur igidlərə bənzəyir:", options:["Kiş kəndinin əhalisi","Qaratəpə dağı","Qalanın möhkəm divarları","Qala düzü"], answer:"C" },
  { id:19, textId:"informativ", subject:"Azərbaycan dili", text:"Mətni məntiqi sonluqla tamamlayın.", options:["bəhs etmişlər.","etiraz etmişlər.","razılaşmışlar.","qənaətə gəlmişlər."], answer:"A" },
  { id:20, textId:"informativ", subject:"Azərbaycan dili", text:"Mətndə bəhsi keçməyən mövzu hansıdır?", options:["Qala divarlarının möhkəmliyi","Qalanın görünüşü","Qalada aşkar olunan əşyalar","Qalanın adının mənası"], answer:"D" },
  { id:21, textId:"informativ", subject:"Azərbaycan dili", text:"Mətndə hansı sualın cavabı yoxdur?", options:["Gələrsən-Görərsən qalası haradadır?","Gələrsən-Görərsən qalası nə zaman inşa olunmuşdur?","Kiş kəndi harada yerləşir?","Qalanın Qaratəpə dağının üstündə salınmasında məqsəd nə olmuşdur?"], answer:"B" },
  { id:22, textId:"informativ", subject:"Azərbaycan dili", text:"Mətni hansı yarımbaşlıqlara ayırmaq olar?\n1. Nadir şahın həyatı\n2. Qalanın tikilmə tarixi\n3. Qala uğrunda gedən döyüşlər\n4. Qalanın əzmkarlığı", options:["1, 3","2, 4","1, 2","3, 4"], answer:"B" },
  { id:23, textId:"informativ", subject:"Azərbaycan dili", text:"Verilmiş hadisənin səbəbi hansıdır?\n\n«Düşmən hücum edən zaman əhali qalaya sığınırdı.»", options:["Çünki qala yüksəklikdə yerləşirdi.","Çünki Şəki şəhəri qala divarları ilə əhatə olunmamışdı.","Çünki düşmən qalaya daxil ola bilmirdi.","Çünki xan insanların qalaya toplanmasını əmr etmişdi."], answer:"B" },
  { id:24, textId:"informativ", subject:"Azərbaycan dili", text:"Mətnə əsasən Gələrsən-Görərsən qalasını seyr etdikdə insanın təsəvvüründə nələr canlanır?", options:["Şəkinin səfalı təbiəti","Şah və xanların dövrü","Məzlum insanlar","Amansız savaşlar"], answer:"D" },
  { id:25, textId:"informativ", subject:"Azərbaycan dili", text:"Mətnə əsasən hansı doğrudur?", options:["Gələrsən-Görərsən qalası Şamaxıda yerləşir.","Qala çökəklikdə tikilmişdir.","Kiş kəndi ilə Şəki arasındakı ərazi Qala düzü adlanır.","Gələrsən-Görərsən qalasının tikilmə tarixi qeyri-məlumdur."], answer:"D" },
  { id:26, textId:"informativ", subject:"Azərbaycan dili", text:"Gələrsən-Görərsən qalasının yerləşdiyi yer haqqında məlumat mətnin hansı hissəsinə aiddir?", options:["Giriş","Əsas","Nəticə","Heç biri"], answer:"A" },
  { id:27, textId:"informativ", subject:"Azərbaycan dili", text:"Nadir şah Hacı Çələbi xandan nəyi tələb etmişdi?", options:["Ordusunu gücləndirməyi","Qalanın təslim edilməsini","Düşmənlə birləşməyi","Diplomatik münasibət qurmağı"], answer:"B" },
  { id:28, textId:"informativ", subject:"Azərbaycan dili", text:"Biri mətndəki fərqləndirilmiş sözü (nəhəng) əvəz edə bilər:", options:["iri","uca","hündür","təmtəraqlı"], answer:"B" },
  { id:29, textId:"informativ", subject:"Azərbaycan dili", text:"Şəki qalasının müdafiəçiləri hansı xüsusiyyətlərlə yadda qalmışdır?", options:["Qorxu və zəiflik","Cəsarət və mətanət","Xəyanət və hiyləgərlik","Nizamsızlıq və tabesizlik"], answer:"B" },
  { id:30, textId:"informativ", subject:"Azərbaycan dili", text:"Mətnə əsasən Nadir şahla bağlı deyilən fikirlərdən biri səhvdir:", options:["Hacı Çələbiyə hədə-qorxu gəlmişdir.","30 minlik qoşunu ilə Şəkiyə hücum etmişdir.","Çələbiyə məktub yazaraq qalanı təslim etməsini tələb etmişdir.","Şəki hakimindən qorxub geri çəkilmişdir."], answer:"D" },
  // Riyaziyyat sualları 31-60
  { id:31, textId:null, subject:"Riyaziyyat", text:"61 ədədini 3 dəfə ardıcıl yazdıqda alınan ədədin minlik mərtəbə qiyməti neçədir?", options:["1 000","6 000","6","600"], answer:"A" },
  { id:32, textId:null, subject:"Riyaziyyat", text:"2 355-dən 265 vahid kiçik ədədlə 588-in cəmi neçəyə bərabərdir?", options:["2 090","2 678","2 943","3 208"], answer:"B" },
  { id:33, textId:null, subject:"Riyaziyyat", text:"Hesablayın və müqayisə edin.\n\n6 325 · 3  □  2 164 · 9", options:[">","<","=","≈"], answer:"B" },
  { id:34, textId:null, subject:"Riyaziyyat", text:"Əməllər ardıcıllığını müəyyən edin.\n\n(16 + (80 : 2 − 35)) · 3", options:["  :  −  +  ·","  :  :  −  +","  ·  :  +  −","  −  ·  +"], answer:"A" },
  { id:35, textId:null, subject:"Riyaziyyat", text:"Yük maşınında 35 yeşik, hər yeşikdə 16 detal var. Yük maşınında cəmi neçə detal var?", options:["430","460","530","560"], answer:"D" },
  { id:36, textId:null, subject:"Riyaziyyat", text:"AOC bucağı 40°, COD və DOB bucaqları bir-birinə bərabər olarsa, DOB bucağının dərəcə ölçüsünü tapın.", options:["140°","120°","70°","60°"], answer:"C" },
  { id:37, textId:null, subject:"Riyaziyyat", text:"16/18 kəsrini ixtisar etsək, hansı kəsr alınır?", options:["8/9","6/9","4/6","8/12"], answer:"A" },
  { id:38, textId:null, subject:"Riyaziyyat", text:"Hansı variantdakı məbləğ 0,8 manata bərabərdir?", options:["A variantı (10q+20q+50q)","B variantı (20q+20q+10q+10q)","C variantı (10q+10q+10q+10q+10q+10q+10q+10q)","D variantı (50q+10q+10q)"], answer:"C" },
  { id:39, textId:null, subject:"Riyaziyyat", text:"Parkda hər 8 m-dən bir skamya yerləşdirdilər. Cəmi 12 skamya yerləşdirilibsə, ilk və son skamya arasındakı məsafə nə qədərdir?", options:["96 m","100 m","88 m","84 m"], answer:"C" },
  { id:40, textId:null, subject:"Riyaziyyat", text:"a = 7 olarsa, (16 555 : a) + 2 354 ifadəsinin qiyməti neçəyə bərabərdir?", options:["4 705","5 719","2 365","4 719"], answer:"D" },
  { id:41, textId:null, subject:"Riyaziyyat", text:"Çevrənin daxilinə çəkilmiş bərabərtərəfli üçbucağın perimetri 24 sm olarsa, çevrənin diametrini tapın.", options:["12 sm","6 sm","8 sm","16 sm"], answer:"C" },
  { id:42, textId:null, subject:"Riyaziyyat", text:"Dairəvi diaqramda 4 ay ərzindəki günəşli günlər verilmişdir: may=20, iyun=25, iyul=24, avqust=28.\nHansı ay günəşli günlərin sayı daha çoxdur?", options:["may","iyun","iyul","avqust"], answer:"D" },
  { id:43, textId:null, subject:"Riyaziyyat", text:"Yay aylarında cəmi neçə gün günəşli gün olub? (may=20, iyun=25, iyul=24, avqust=28)", options:["97","73","77","92"], answer:"A" },
  { id:44, textId:null, subject:"Riyaziyyat", text:"May və iyun aylarındakı günəşli günlərin sayı avqust ayındakı günəşli günlərin sayından nə qədər çoxdur?", options:["17","33","23","27"], answer:"A" },
  { id:45, textId:null, subject:"Riyaziyyat", text:"65 565-dən kiçik, minlik mərtəbə qiyməti 4 000 olan ən böyük tək ədəd neçədir?", options:["65 563","65 463","68 563","64 999"], answer:"A" },
  { id:46, textId:null, subject:"Riyaziyyat", text:"Hansı ədədi onminliklərə qədər yuvarlaqlaşdırdıqda özündən kiçik ədəd alınır?", options:["31 645","26 741","68 336","45 314"], answer:"D" },
  { id:47, textId:null, subject:"Riyaziyyat", text:"6, 3, 8, 1, 7 rəqəmlərindən bir dəfə istifadə etməklə düzələn ən kiçik beşrəqəmli ədədlə ən böyük dördrəqəmli ədədin cəmini tapın.", options:["72 580","22 441","21 341","101 309"], answer:"B" },
  { id:48, textId:null, subject:"Riyaziyyat", text:"Verilən ədədlərdən hansı nə 3-ə, nə də 5-ə qalıqsız bölünür?", options:["34 685","26 115","13 654","41 991"], answer:"C" },
  { id:49, textId:null, subject:"Riyaziyyat", text:"İki ağacdan 125 kq alma yığdılar. Birinci ağacdan ikinci ağacdakından 15 kq çox alma yığılmışdır. İkinci ağacdan nə qədər alma yığıldı?", options:["55 kq","70 kq","40 kq","65 kq"], answer:"C" },
  { id:50, textId:null, subject:"Riyaziyyat", text:"Tənliyi həll edin.\n\n36 · x = 300 − 12", options:["3","13","6","8"], answer:"D" },
  { id:51, textId:null, subject:"Riyaziyyat", text:"Koordinat şəbəkəsindəki C nöqtəsinin koordinatları hansılardır?", options:["(0; 2)","(2; 0)","(1; 2)","(2; 1)"], answer:"D" },
  { id:52, textId:null, subject:"Riyaziyyat", text:"Koordinat başlanğıcından 4 vahid yuxarı, 8 vahid sağda yerləşən nöqtə hansıdır?", options:["B","D","E","F"], answer:"B" },
  { id:53, textId:null, subject:"Riyaziyyat", text:"Verilən saatdan (17:15) 4 saat sonra başlayan film 2 saat 10 dəq davam etdi. Film saat neçədə bitdi?", options:["22:25","23:25","21:15","20:15"], answer:"B" },
  { id:54, textId:null, subject:"Riyaziyyat", text:"Hansı variantda kubun açılışı düzgün verilmişdir?", options:["A variantı","B variantı","C variantı","D variantı (xaç formalı)"], answer:"D" },
  { id:55, textId:null, subject:"Riyaziyyat", text:"1 kq çiyələyin qiyməti 4 manat 20 qəpikdir. 3 kq çiyələk alan alıcı kassaya nə qədər pul ödəməlidir?", options:["8,4 manat","8,6 manat","12,5 manat","12,6 manat"], answer:"D" },
  { id:56, textId:null, subject:"Riyaziyyat", text:"Piktoqrama əsasən hansı gün satılan unun miqdarı 4 gün ərzində satılan unun miqdarının 1/7 hissəsinə bərabərdir?\n(B.ertəsi=7kq, Ç.axşamı=5kq, Çərşənbə=6kq, C.axşamı=10kq; hər kvadrat=2kq)", options:["bazar ertəsi","çərşənbə axşamı","çərşənbə","cümə axşamı"], answer:"A" },
  { id:57, textId:null, subject:"Riyaziyyat", text:"Sahəsi 64 dm² olan kvadratın perimetri neçə metrdir?", options:["1,6 m","16 m","3,2 m","32 m"], answer:"C" },
  { id:58, textId:null, subject:"Riyaziyyat", text:"A məntəqəsindən eyni zamanda eyni istiqamətdə sürətləri 75 km/saat və 84 km/saat olan iki avtomobil yola düşdü. 3 saat sonra onlar arasındakı məsafə neçə km olar?", options:["27 km","25 km","30 km","20 km"], answer:"A", isOpen:true },
  { id:59, textId:null, subject:"Riyaziyyat", text:"Hesablayın.\n\n9,58 − 4,34 + 1,2", options:["6,44","5,24","6,04","7,44"], answer:"A", isOpen:true },
  { id:60, textId:null, subject:"Riyaziyyat", text:"1/5 m neçə santimetrdir?", options:["20 sm","25 sm","15 sm","5 sm"], answer:"A", isOpen:true },
];

const TOTAL_TIME = 2 * 60 * 60;

function formatTime(s) {
  const h = Math.floor(s/3600), m = Math.floor((s%3600)/60), sec = s%60;
  return `${String(h).padStart(2,"0")}:${String(m).padStart(2,"0")}:${String(sec).padStart(2,"0")}`;
}

function RenderContent({ content }) {
  return (
    <div>
      {content.map((block, i) => {
        if (block.type === "p" || block.type === "num") {
          if (block.parts) {
            return (
              <p key={i} style={{ margin:"0 0 10px", lineHeight:"1.8", color:"#e8e8e8", fontSize:"15px" }}>
                {block.n && <strong style={{color:"#ffd700",marginRight:"6px"}}>{block.n}</strong>}
                {block.text}
                {block.parts.map((p,j) => (
                  p.underline
                    ? <span key={j} style={{ textDecoration:"underline", fontWeight:"bold", color:"#ff6b6b" }}>{p.t}</span>
                    : <span key={j}>{p.t}</span>
                ))}
              </p>
            );
          }
          return (
            <p key={i} style={{ margin:"0 0 10px", lineHeight:"1.8", color:"#e8e8e8", fontSize:"15px" }}>
              {block.n && <strong style={{color:"#ffd700",marginRight:"6px"}}>{block.n}</strong>}
              {block.text}
            </p>
          );
        }
        if (block.type === "dialog") {
          return (
            <p key={i} style={{
              margin:"0 0 10px", lineHeight:"1.8", color:"#c8e6ff", fontSize:"15px",
              paddingLeft:"16px", borderLeft:"3px solid #4a9eff", fontStyle:"italic"
            }}>
              {block.text}
            </p>
          );
        }
        return null;
      })}
    </div>
  );
}

export default function App() {
  const [phase, setPhase] = useState("start");
  const [answers, setAnswers] = useState({});
  const [timeLeft, setTimeLeft] = useState(TOTAL_TIME);
  const [currentQ, setCurrentQ] = useState(0);
  const [showText, setShowText] = useState(false);
  const timerRef = useRef(null);
  const topRef = useRef(null);

  useEffect(() => {
    if (phase === "exam") {
      timerRef.current = setInterval(() => {
        setTimeLeft(t => {
          if (t <= 1) { clearInterval(timerRef.current); setPhase("result"); return 0; }
          return t - 1;
        });
      }, 1000);
    }
    return () => clearInterval(timerRef.current);
  }, [phase]);

  const handleAnswer = (qId, opt) => setAnswers(prev => ({ ...prev, [qId]: opt }));

  const goTo = (i) => {
    setCurrentQ(i);
    setShowText(false);
    topRef.current?.scrollIntoView({ behavior:"smooth" });
  };

  const handleSubmit = () => { clearInterval(timerRef.current); setPhase("result"); };

  const letters = ["A","B","C","D"];

  // ── RESULTS ──
  if (phase === "result") {
    let correct=0, wrong=0, blank=0;
    const details = questions.map(q => {
      const g = answers[q.id];
      if (!g) { blank++; return {...q, given:g, status:"blank"}; }
      if (g === q.answer) { correct++; return {...q, given:g, status:"correct"}; }
      wrong++;
      return {...q, given:g, status:"wrong"};
    });
    const pct = Math.round(correct/questions.length*100);
    const grade = pct>=85?"Əla":pct>=70?"Yaxşı":pct>=50?"Kafi":"Qeyri-kafi";
    const gc = pct>=85?"#4ade80":pct>=70?"#60a5fa":pct>=50?"#fbbf24":"#f87171";
    const azC = details.filter(d=>d.subject==="Azərbaycan dili"&&d.status==="correct").length;
    const mC = details.filter(d=>d.subject==="Riyaziyyat"&&d.status==="correct").length;
    const usedTime = TOTAL_TIME - timeLeft;
    const uh = Math.floor(usedTime/3600), um = Math.floor((usedTime%3600)/60);

    return (
      <div style={{ minHeight:"100vh", background:"linear-gradient(135deg,#0f2027,#203a43,#2c5364)", fontFamily:"Georgia,serif", padding:"20px" }}>
        <div style={{ maxWidth:"800px", margin:"0 auto" }}>
          <div style={{ background:"rgba(255,255,255,0.05)", border:"1px solid rgba(255,215,0,0.3)", borderRadius:"20px", padding:"35px", marginBottom:"20px", textAlign:"center" }}>
            <div style={{ fontSize:"52px" }}>🏆</div>
            <h2 style={{ color:"#ffd700", margin:"8px 0 4px", fontSize:"26px" }}>İmtahan Başa Çatdı!</h2>
            <p style={{ color:"#a8d8ea", margin:0 }}>4-cü sinif · Ümumi Monitorinq Sınaq – 1</p>
            <p style={{ color:"#888", fontSize:"13px", marginTop:"6px" }}>Sərf edilən vaxt: {uh} saat {um} dəq</p>
          </div>

          <div style={{ display:"grid", gridTemplateColumns:"repeat(3,1fr)", gap:"12px", marginBottom:"16px" }}>
            {[["✅ Düzgün",correct,"#4ade80"],["❌ Səhv",wrong,"#f87171"],["⬜ Boş",blank,"#94a3b8"]].map(([l,v,c])=>(
              <div key={l} style={{ background:"rgba(255,255,255,0.06)", border:`1px solid ${c}40`, borderRadius:"14px", padding:"18px", textAlign:"center" }}>
                <div style={{ color:c, fontSize:"34px", fontWeight:"bold" }}>{v}</div>
                <div style={{ color:"#aaa", fontSize:"13px", marginTop:"4px" }}>{l}</div>
              </div>
            ))}
          </div>

          <div style={{ background:"rgba(255,255,255,0.06)", borderRadius:"16px", padding:"22px", marginBottom:"16px", textAlign:"center" }}>
            <div style={{ color:"#a8d8ea", marginBottom:"8px" }}>Ümumi Nəticə</div>
            <div style={{ color:gc, fontSize:"52px", fontWeight:"bold" }}>{pct}%</div>
            <div style={{ color:gc, fontSize:"20px" }}>({grade})</div>
            <div style={{ color:"#888", marginTop:"6px" }}>{correct} / {questions.length} sual düzgün</div>
          </div>

          <div style={{ display:"grid", gridTemplateColumns:"1fr 1fr", gap:"12px", marginBottom:"16px" }}>
            {[["📖 Azərbaycan dili",azC,30],["🔢 Riyaziyyat",mC,30]].map(([s,sc,tot])=>(
              <div key={s} style={{ background:"rgba(255,255,255,0.06)", borderRadius:"14px", padding:"18px", textAlign:"center" }}>
                <div style={{ color:"#ffd700", fontSize:"13px", marginBottom:"6px" }}>{s}</div>
                <div style={{ color:"#fff", fontSize:"26px", fontWeight:"bold" }}>{sc}/{tot}</div>
                <div style={{ color:"#888", fontSize:"12px" }}>{Math.round(sc/tot*100)}%</div>
                <div style={{ background:"rgba(255,255,255,0.1)", borderRadius:"10px", height:"7px", marginTop:"10px", overflow:"hidden" }}>
                  <div style={{ height:"100%", width:`${sc/tot*100}%`, background:"linear-gradient(90deg,#ffd700,#ff8c00)", borderRadius:"10px" }} />
                </div>
              </div>
            ))}
          </div>

          {/* Detailed breakdown */}
          <div style={{ background:"rgba(255,255,255,0.04)", border:"1px solid rgba(255,255,255,0.08)", borderRadius:"16px", padding:"22px", marginBottom:"16px" }}>
            <h3 style={{ color:"#ffd700", margin:"0 0 16px", fontSize:"17px" }}>Cavabların Təhlili</h3>
            <div style={{ display:"flex", flexWrap:"wrap", gap:"7px" }}>
              {details.map(d=>(
                <div key={d.id} title={`S${d.id}: Siz: ${d.given||"–"} | Düzgün: ${d.answer}`} style={{
                  width:"40px", height:"40px", borderRadius:"9px",
                  display:"flex", alignItems:"center", justifyContent:"center",
                  fontSize:"12px", fontWeight:"bold", cursor:"default",
                  background: d.status==="correct"?"rgba(74,222,128,0.2)":d.status==="wrong"?"rgba(248,113,113,0.2)":"rgba(148,163,184,0.12)",
                  border:`2px solid ${d.status==="correct"?"#4ade80":d.status==="wrong"?"#f87171":"#94a3b8"}`,
                  color: d.status==="correct"?"#4ade80":d.status==="wrong"?"#f87171":"#94a3b8"
                }}>{d.id}</div>
              ))}
            </div>
            <p style={{ color:"#555", fontSize:"11px", marginTop:"10px" }}>Üzərinə gəlin → cavabı görün</p>
          </div>

          {/* Wrong answers list */}
          {wrong > 0 && (
            <div style={{ background:"rgba(248,113,113,0.06)", border:"1px solid rgba(248,113,113,0.2)", borderRadius:"16px", padding:"22px", marginBottom:"16px" }}>
              <h3 style={{ color:"#f87171", margin:"0 0 14px", fontSize:"17px" }}>❌ Səhv Cavablar</h3>
              {details.filter(d=>d.status==="wrong").map(d=>(
                <div key={d.id} style={{ borderBottom:"1px solid rgba(255,255,255,0.06)", paddingBottom:"10px", marginBottom:"10px" }}>
                  <div style={{ color:"#ccc", fontSize:"13px", marginBottom:"4px" }}>
                    <span style={{ color:"#ffd700", fontWeight:"bold" }}>S{d.id}.</span> {d.text.length > 80 ? d.text.slice(0,80)+"…" : d.text}
                  </div>
                  <div style={{ display:"flex", gap:"16px", fontSize:"13px" }}>
                    <span style={{ color:"#f87171" }}>Siz: {d.given}</span>
                    <span style={{ color:"#4ade80" }}>Düzgün: {d.answer}</span>
                  </div>
                </div>
              ))}
            </div>
          )}

          <button onClick={()=>{ setAnswers({}); setTimeLeft(TOTAL_TIME); setCurrentQ(0); setShowText(false); setPhase("start"); }} style={{
            width:"100%", background:"linear-gradient(135deg,#ffd700,#ff8c00)", color:"#000",
            border:"none", borderRadius:"14px", padding:"16px", fontSize:"17px",
            fontWeight:"bold", cursor:"pointer"
          }}>🔄 Yenidən Başla</button>
        </div>
      </div>
    );
  }

  // ── START ──
  if (phase === "start") {
    return (
      <div style={{ minHeight:"100vh", background:"linear-gradient(135deg,#0f2027,#203a43,#2c5364)", display:"flex", flexDirection:"column", alignItems:"center", justifyContent:"center", fontFamily:"Georgia,serif", padding:"20px" }}>
        <div style={{ background:"rgba(255,255,255,0.05)", border:"1px solid rgba(255,215,0,0.2)", borderRadius:"20px", padding:"50px 40px", maxWidth:"580px", width:"100%", textAlign:"center" }}>
          <div style={{ fontSize:"58px", marginBottom:"8px" }}>📚</div>
          <h1 style={{ color:"#ffd700", fontSize:"26px", margin:"0 0 6px" }}>Ümumi Monitorinq Sınaq – 1</h1>
          <p style={{ color:"#a8d8ea", margin:"0 0 30px" }}>4-cü sinif · ORTA səviyyə</p>
          <div style={{ display:"grid", gridTemplateColumns:"1fr 1fr", gap:"12px", marginBottom:"32px" }}>
            {[["⏱️ Müddət","2 saat"],["📝 Sual sayı","60 sual"],["📖 Azərbaycan dili","30 sual (2 mətn)"],["🔢 Riyaziyyat","30 sual"]].map(([k,v])=>(
              <div key={k} style={{ background:"rgba(255,255,255,0.07)", borderRadius:"12px", padding:"14px", border:"1px solid rgba(255,215,0,0.15)" }}>
                <div style={{ color:"#888", fontSize:"12px", marginBottom:"3px" }}>{k}</div>
                <div style={{ color:"#fff", fontSize:"16px", fontWeight:"bold" }}>{v}</div>
              </div>
            ))}
          </div>
          <div style={{ background:"rgba(168,216,234,0.08)", borderRadius:"12px", padding:"14px", marginBottom:"28px", textAlign:"left" }}>
            <p style={{ color:"#a8d8ea", fontSize:"13px", margin:"0 0 6px", fontWeight:"bold" }}>📌 Mətn haqqında</p>
            <p style={{ color:"#888", fontSize:"13px", margin:0 }}>Azərbaycan dili bölməsindəki hər sualda "Mətni oxu" düyməsi ilə əlaqəli mətni tam oxuya bilərsiniz.</p>
          </div>
          <button onClick={()=>setPhase("exam")} style={{ background:"linear-gradient(135deg,#ffd700,#ff8c00)", color:"#000", border:"none", borderRadius:"50px", padding:"16px 50px", fontSize:"18px", fontWeight:"bold", cursor:"pointer", boxShadow:"0 4px 20px rgba(255,215,0,0.35)" }}>
            İmtahana Başla →
          </button>
        </div>
      </div>
    );
  }

  // ── EXAM ──
  const q = questions[currentQ];
  const isAz = q.subject === "Azərbaycan dili";
  const textData = q.textId ? texts[q.textId] : null;
  const answeredCount = Object.keys(answers).length;
  const timerColor = timeLeft<600?"#f87171":timeLeft<1800?"#fbbf24":"#4ade80";

  // group for nav
  const azQs = questions.filter(x=>x.subject==="Azərbaycan dili");
  const mathQs = questions.filter(x=>x.subject==="Riyaziyyat");

  return (
    <div style={{ minHeight:"100vh", background:"linear-gradient(135deg,#0f2027,#203a43,#2c5364)", fontFamily:"Georgia,serif" }}>
      {/* Sticky top bar */}
      <div ref={topRef} style={{ background:"rgba(0,0,0,0.5)", backdropFilter:"blur(12px)", padding:"10px 18px", display:"flex", alignItems:"center", justifyContent:"space-between", position:"sticky", top:0, zIndex:100, borderBottom:"1px solid rgba(255,255,255,0.08)" }}>
        <div style={{ color:"#ffd700", fontWeight:"bold", fontSize:"14px" }}>{q.subject}</div>
        <div style={{ color:timerColor, fontWeight:"bold", fontSize:"20px", fontFamily:"monospace", letterSpacing:"2px" }}>⏱ {formatTime(timeLeft)}</div>
        <div style={{ color:"#a8d8ea", fontSize:"13px" }}>{answeredCount}/{questions.length}</div>
      </div>
      {/* Progress bar */}
      <div style={{ height:"3px", background:"rgba(255,255,255,0.08)" }}>
        <div style={{ height:"100%", width:`${answeredCount/questions.length*100}%`, background:"linear-gradient(90deg,#ffd700,#ff8c00)", transition:"width 0.3s" }} />
      </div>

      <div style={{ maxWidth:"760px", margin:"0 auto", padding:"18px" }}>

        {/* TEXT PANEL */}
        {textData && (
          <div style={{ marginBottom:"14px" }}>
            <button onClick={()=>setShowText(v=>!v)} style={{
              width:"100%", padding:"13px 18px", background: showText ? "rgba(255,215,0,0.15)" : "rgba(255,255,255,0.06)",
              border:`1px solid ${showText ? "#ffd700" : "rgba(255,255,255,0.15)"}`,
              borderRadius:"14px", color: showText ? "#ffd700" : "#a8d8ea",
              fontSize:"15px", cursor:"pointer", display:"flex", alignItems:"center", justifyContent:"space-between", fontFamily:"Georgia,serif"
            }}>
              <span>📖 {textData.title}</span>
              <span style={{ fontSize:"12px", opacity:0.7 }}>{showText ? "▲ Bağla" : "▼ Mətni oxu"}</span>
            </button>

            {showText && (
              <div style={{
                background:"rgba(255,255,255,0.04)", border:"1px solid rgba(255,215,0,0.2)",
                borderRadius:"0 0 14px 14px", padding:"22px", marginTop:"-2px"
              }}>
                <h3 style={{ color:"#ffd700", margin:"0 0 16px", fontSize:"16px", textAlign:"center", letterSpacing:"0.5px" }}>
                  {textData.title}
                </h3>
                <RenderContent content={textData.content} />
                {textData.source && (
                  <p style={{ color:"#ff9f43", fontStyle:"italic", textAlign:"center", marginTop:"16px", fontSize:"14px" }}>
                    {textData.source}
                  </p>
                )}
              </div>
            )}
          </div>
        )}

        {/* QUESTION CARD */}
        <div style={{ background:"rgba(255,255,255,0.05)", border:"1px solid rgba(255,215,0,0.2)", borderRadius:"16px", padding:"22px", marginBottom:"14px" }}>
          <div style={{ display:"flex", justifyContent:"space-between", alignItems:"center", marginBottom:"12px" }}>
            <span style={{
              background: isAz ? "rgba(168,216,234,0.15)" : "rgba(255,215,0,0.15)",
              color: isAz ? "#a8d8ea" : "#ffd700",
              padding:"3px 12px", borderRadius:"20px", fontSize:"12px"
            }}>{q.subject}</span>
            <span style={{ color:"#666", fontSize:"13px" }}>Sual {q.id} / {questions.length}</span>
          </div>
          <p style={{ color:"#fff", fontSize:"15px", lineHeight:"1.75", margin:0, whiteSpace:"pre-line" }}>
            {q.text}
          </p>
        </div>

        {/* OPTIONS */}
        <div style={{ display:"flex", flexDirection:"column", gap:"9px", marginBottom:"18px" }}>
          {q.options.map((opt,i)=>{
            const letter = letters[i];
            const sel = answers[q.id] === letter;
            return (
              <button key={i} onClick={()=>handleAnswer(q.id,letter)} style={{
                background: sel ? "rgba(255,215,0,0.18)" : "rgba(255,255,255,0.05)",
                border:`2px solid ${sel?"#ffd700":"rgba(255,255,255,0.1)"}`,
                borderRadius:"13px", padding:"13px 16px", color: sel?"#ffd700":"#ddd",
                fontSize:"15px", textAlign:"left", cursor:"pointer",
                display:"flex", alignItems:"center", gap:"12px", transition:"all 0.15s",
                fontFamily:"Georgia,serif"
              }}>
                <span style={{
                  width:"28px", height:"28px", borderRadius:"50%", flexShrink:0,
                  background: sel?"#ffd700":"rgba(255,255,255,0.1)",
                  color: sel?"#000":"#888", display:"flex", alignItems:"center",
                  justifyContent:"center", fontWeight:"bold", fontSize:"13px"
                }}>{letter}</span>
                {opt}
              </button>
            );
          })}
        </div>

        {/* NAV BUTTONS */}
        <div style={{ display:"flex", gap:"10px", marginBottom:"22px" }}>
          <button onClick={()=>goTo(Math.max(0,currentQ-1))} disabled={currentQ===0} style={{
            flex:1, padding:"12px", borderRadius:"12px", border:"1px solid rgba(255,255,255,0.12)",
            background:"rgba(255,255,255,0.05)", color:currentQ===0?"#444":"#fff",
            cursor:currentQ===0?"not-allowed":"pointer", fontSize:"15px", fontFamily:"Georgia,serif"
          }}>← Geri</button>
          <button onClick={()=>goTo(Math.min(questions.length-1,currentQ+1))} disabled={currentQ===questions.length-1} style={{
            flex:1, padding:"12px", borderRadius:"12px", border:"1px solid rgba(255,255,255,0.12)",
            background:"rgba(255,255,255,0.05)", color:currentQ===questions.length-1?"#444":"#fff",
            cursor:currentQ===questions.length-1?"not-allowed":"pointer", fontSize:"15px", fontFamily:"Georgia,serif"
          }}>İrəli →</button>
        </div>

        {/* QUESTION GRID */}
        <div style={{ background:"rgba(255,255,255,0.03)", border:"1px solid rgba(255,255,255,0.07)", borderRadius:"14px", padding:"16px", marginBottom:"16px" }}>
          <div style={{ color:"#888", fontSize:"12px", marginBottom:"10px" }}>📖 Azərbaycan dili (1–30)</div>
          <div style={{ display:"flex", flexWrap:"wrap", gap:"6px", marginBottom:"14px" }}>
            {azQs.map(qq=>{
              const idx = questions.findIndex(x=>x.id===qq.id);
              const isCur = idx===currentQ;
              const isAns = !!answers[qq.id];
              return (
                <button key={qq.id} onClick={()=>goTo(idx)} style={{
                  width:"34px", height:"34px", borderRadius:"7px", border:"none",
                  background: isCur?"#ffd700":isAns?"rgba(74,222,128,0.25)":"rgba(255,255,255,0.07)",
                  color: isCur?"#000":isAns?"#4ade80":"#777",
                  fontWeight:"bold", fontSize:"11px", cursor:"pointer",
                  outline: isCur?"2px solid #ffd700":"none"
                }}>{qq.id}</button>
              );
            })}
          </div>
          <div style={{ color:"#888", fontSize:"12px", marginBottom:"10px" }}>🔢 Riyaziyyat (31–60)</div>
          <div style={{ display:"flex", flexWrap:"wrap", gap:"6px" }}>
            {mathQs.map(qq=>{
              const idx = questions.findIndex(x=>x.id===qq.id);
              const isCur = idx===currentQ;
              const isAns = !!answers[qq.id];
              return (
                <button key={qq.id} onClick={()=>goTo(idx)} style={{
                  width:"34px", height:"34px", borderRadius:"7px", border:"none",
                  background: isCur?"#ffd700":isAns?"rgba(74,222,128,0.25)":"rgba(255,255,255,0.07)",
                  color: isCur?"#000":isAns?"#4ade80":"#777",
                  fontWeight:"bold", fontSize:"11px", cursor:"pointer",
                  outline: isCur?"2px solid #ffd700":"none"
                }}>{qq.id}</button>
              );
            })}
          </div>
        </div>

        <button onClick={handleSubmit} style={{
          width:"100%", padding:"15px", background:"linear-gradient(135deg,#dc2626,#b91c1c)",
          color:"#fff", border:"none", borderRadius:"13px", fontSize:"16px",
          fontWeight:"bold", cursor:"pointer", fontFamily:"Georgia,serif"
        }}>✔ İmtahanı Bitir</button>
      </div>
    </div>
  );
}
