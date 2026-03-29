\# 🎤 Proqramlaşdırma Müsahibə Sualları



> Bu sənəd proqramlaşdırma müsahiblərində ən çox soruşulan texniki və davranış suallarını əhatə edir.



\---



\## 🧩 Alqoritm / Data Structure Sualları



\### Ən Tez-tez Soruşulanlar (LeetCode Easy-Medium)



Bu kateqoriyalar müsahibələrdə ən çox çıxır:



| Kateqoriya | Vaciblik | Hansı Şirkətlər |

|-----------|---------|----------------|

| Arrays \& Hashing | ⭐⭐⭐⭐⭐ | Hamısı |

| Two Pointers | ⭐⭐⭐⭐⭐ | Hamısı |

| Sliding Window | ⭐⭐⭐⭐ | Google, Meta, Amazon |

| Stack \& Queue | ⭐⭐⭐⭐ | Hamısı |

| Binary Search | ⭐⭐⭐⭐ | Google, Microsoft |

| Linked List | ⭐⭐⭐⭐ | Hamısı |

| Trees \& BFS/DFS | ⭐⭐⭐⭐⭐ | Hamısı |

| Graphs | ⭐⭐⭐ | Google, Meta |

| Dynamic Programming | ⭐⭐⭐⭐ | Amazon, Google |

| Greedy Algorithms | ⭐⭐⭐ | Hamısı |



\### Məşq üçün Qaynaqlar



\- \[NeetCode 150](https://neetcode.io/roadmap) — Ən vacib 150 problem, kateqoriyalar üzrə ⭐

\- \[LeetCode Top Interview 150](https://leetcode.com/studyplan/top-interview-150/) — Standart problem set

\- \[Blind 75](https://leetcode.com/discuss/general-discussion/460599/blind-75-leetcode-questions) — Klassik 75 problem



\---



\## 🖥️ Texniki Suallar — JavaScript / Frontend



<details>

<summary><b>JavaScript-də <code>var</code>, <code>let</code>, <code>const</code> arasındakı fərq nədir?</b></summary>



\- \*\*`var`\*\*: Function-scoped, hoisting olur, yenidən təyin edilə bilər

\- \*\*`let`\*\*: Block-scoped, hoisting olmaz (TDZ var), yenidən təyin edilə bilər

\- \*\*`const`\*\*: Block-scoped, yenidən təyin edilə bilməz, amma obyekt/array mutasiyası mümkündür



```javascript

// var hoisting nümunəsi

console.log(x); // undefined (xəta deyil!)

var x = 5;



// let — TDZ (Temporal Dead Zone)

console.log(y); // ReferenceError!

let y = 5;



// const — primitiv dəyər dəyişdirilmir

const z = 10;

z = 20; // TypeError!



// amma const ilə obyekt dəyişdirilə bilər

const obj = { a: 1 };

obj.a = 2; // ✅ Bu mümkündür

```



</details>



<details>

<summary><b>Closure nədir?</b></summary>



Closure — bir funksiyanın özünü əhatə edən leksik mühitə (scope-a) istinad etməsidir. Funksiya icra olunduqdan sonra da outer scope-dakı dəyişkənlərə çata bilir.



```javascript

function counter() {

&#x20; let count = 0; // bu dəyişkən "captured" olunur

&#x20; return {

&#x20;   increment: () => ++count,

&#x20;   getCount: () => count

&#x20; };

}



const c = counter();

c.increment(); // 1

c.increment(); // 2

c.getCount();  // 2

// count dəyişkənə xaricdən çatmaq mümkün deyil — encapsulation

```



\*\*Nə üçün vacibdir:\*\* Module pattern, event handlers, memoization, private state.



</details>



<details>

<summary><b>Promise, async/await nədir?</b></summary>



JavaScript asinxron əməliyyatları idarə etmək üçün 3 yol:



\*\*Callback (köhnə):\*\*

```javascript

fetch(url, function(data) {

&#x20; process(data, function(result) {

&#x20;   // callback hell

&#x20; });

});

```



\*\*Promise:\*\*

```javascript

fetch(url)

&#x20; .then(data => process(data))

&#x20; .then(result => console.log(result))

&#x20; .catch(err => console.error(err));

```



\*\*Async/Await (müasir, tövsiyə edilir):\*\*

```javascript

async function getData() {

&#x20; try {

&#x20;   const data = await fetch(url);

&#x20;   const result = await process(data);

&#x20;   return result;

&#x20; } catch (err) {

&#x20;   console.error(err);

&#x20; }

}

```



</details>



<details>

<summary><b>Event Loop nədir?</b></summary>



JavaScript tək axınlı (single-threaded) dildir — eyni anda yalnız bir iş görür. Lakin asinxron əməliyyatları (setTimeout, API çağrısı) Event Loop sayəsində idarə edir:



1\. \*\*Call Stack\*\* — hazırda işləyən funksiyalar

2\. \*\*Web API\*\* — setTimeout, fetch → brauzer burada idarə edir

3\. \*\*Callback Queue\*\* — hazır olan callback-lər gözləyir

4\. \*\*Event Loop\*\* — Call Stack boşaldıqda Queue-dən götürüb Stack-ə atır



```javascript

console.log("1");           // Call Stack

setTimeout(() => console.log("2"), 0); // Web API → Queue

console.log("3");           // Call Stack

// Çıxış: 1, 3, 2

```



</details>



\---



\## 🐍 Texniki Suallar — Python



<details>

<summary><b>Python-da <code>list</code> və <code>tuple</code> fərqi nədir?</b></summary>



| Xüsusiyyət | List | Tuple |

|-----------|------|-------|

| Dəyişdirilir? | ✅ Bəli (mutable) | ❌ Xeyr (immutable) |

| Sintaksis | `\[1, 2, 3]` | `(1, 2, 3)` |

| Sürət | Yavaş | Sürətli |

| Yaddaş | Çox | Az |

| Həsh? | ❌ | ✅ (dict key ola bilər) |



\*\*Nə zaman tuple istifadə et:\*\* Dəyişməyəcək məlumatlar üçün (koordinatlar, rənglər, verilənlər bazası cərgələri).



</details>



<details>

<summary><b>Decorator nədir?</b></summary>



Decorator — bir funksiyanı başqa bir funksiyaya "bürüyən" dizayn patternidir. Funksiyaya davranış əlavə etmək üçün istifadə olunur.



```python

def timer(func):

&#x20;   import time

&#x20;   def wrapper(\*args, \*\*kwargs):

&#x20;       start = time.time()

&#x20;       result = func(\*args, \*\*kwargs)

&#x20;       print(f"{func.\_\_name\_\_} {time.time()-start:.4f}s çəkdi")

&#x20;       return result

&#x20;   return wrapper



@timer

def hesabla(n):

&#x20;   return sum(range(n))



hesabla(1000000)

\# Çıxış: hesabla 0.0234s çəkdi

```



\*\*Real istifadə yerləri:\*\* Flask/Django route-ları, autentifikasiya yoxlaması, caching, logging.



</details>



<details>

<summary><b>GIL (Global Interpreter Lock) nədir?</b></summary>



GIL — CPython interpreter-in bir anda yalnız bir Python thread-inin icra olmasına imkan verən mexanizmdir.



\*\*Problemi:\*\* Çox nüvəli prosessoru tam istifadə edə bilmirsən (CPU-bound işlər üçün).



\*\*Həlli:\*\*

\- CPU-bound işlər → `multiprocessing` modul istifadə et (ayrı proseslər)

\- I/O-bound işlər → `asyncio` / `threading` (GIL problem deyil)

\- Python 3.13+ → "free-threaded" mode eksperimental olaraq gəlir



</details>



\---



\## ☕ Texniki Suallar — Java



<details>

<summary><b>OOP-nun 4 əsas prinsipi nədir?</b></summary>



1\. \*\*Encapsulation (Gizlətmə):\*\* Məlumatları `private` saxla, `getter/setter` ilə idarə et

2\. \*\*Inheritance (Miras):\*\* `extends` — alt sinif üst sinfin xüsusiyyətlərini miras alır

3\. \*\*Polymorphism (Çoxbiçimlilik):\*\* Eyni ad, fərqli davranış (Override, Overload)

4\. \*\*Abstraction (Soyutlama):\*\* Abstract class / Interface ilə tətbiqat detallarını gizlət



```java

// Polymorphism nümunəsi

class Shape {

&#x20;   double area() { return 0; }

}

class Circle extends Shape {

&#x20;   double r;

&#x20;   Circle(double r) { this.r = r; }

&#x20;   @Override

&#x20;   double area() { return Math.PI \* r \* r; }

}

class Square extends Shape {

&#x20;   double s;

&#x20;   Square(double s) { this.s = s; }

&#x20;   @Override

&#x20;   double area() { return s \* s; }

}

```



</details>



<details>

<summary><b>Interface və Abstract Class fərqi nədir?</b></summary>



| Xüsusiyyət | Interface | Abstract Class |

|-----------|-----------|----------------|

| Çoxlu miras | ✅ Bəli | ❌ Xeyr |

| Constructor | ❌ Yoxdur | ✅ Var |

| Tətbiq edilmiş metodlar | Java 8+ default var | ✅ Var |

| Dəyişənlər | `public static final` | Hər növ |

| Nə zaman | "nə edir" | "nədir" |



</details>



\---



\## 🗄️ Verilənlər Bazası Sualları



<details>

<summary><b>SQL JOIN növləri nələrdir?</b></summary>



```sql

\-- INNER JOIN: Hər iki cədvəldə uyğun olan sətrlər

SELECT u.name, o.product

FROM users u

INNER JOIN orders o ON u.id = o.user\_id;



\-- LEFT JOIN: Sol cədvəlin hamısı + sağdan uyğun olanlar

SELECT u.name, o.product

FROM users u

LEFT JOIN orders o ON u.id = o.user\_id;

\-- (sifarişi olmayan user-lər də gəlir, o.product = NULL)



\-- RIGHT JOIN: Sağ cədvəlin hamısı + soldan uyğun olanlar

\-- FULL OUTER JOIN: Hər iki cədvəlin hamısı

\-- CROSS JOIN: Karteş hasili (hər sətir hər sətrlə)

```



</details>



<details>

<summary><b>Index nədir, nə vaxt istifadə edilir?</b></summary>



Index — cədvəldəki sorğuların sürətini artırmaq üçün yaradılan məlumat strukturudur (B-tree əsaslı).



```sql

\-- Index yaratmaq

CREATE INDEX idx\_user\_email ON users(email);



\-- Nə vaxt lazımdır:

\-- ✅ Tez-tez WHERE ilə axtarılan sütunlar

\-- ✅ JOIN-lərdə istifadə olunan sütunlar

\-- ✅ ORDER BY sütunları



\-- Nə vaxt lazım deyil:

\-- ❌ Çox az məlumat olan cədvəllər

\-- ❌ Tez-tez INSERT/UPDATE olan cədvəllər (index yavaşladır)

\-- ❌ Boolean (true/false) sütunlar

```



</details>



\---



\## 🏗️ Sistem Dizaynı Sualları (Mid/Senior)



<details>

<summary><b>URL qısaldıcı (bit.ly kimi) necə dizayn edilər?</b></summary>



\*\*Tələblər:\*\*

\- Uzun URL → qısa URL (7 simvol)

\- Yönləndirmə: `bit.ly/abc1234` → orijinal URL



\*\*Həll:\*\*

1\. Qısa kod yaratmaq: Base62 kodlaşdırma (a-z, A-Z, 0-9 = 62 simvol)

2\. 7 simvol = 62^7 = 3.5 trilyon unikal URL

3\. Verilənlər bazası: `short\_code → original\_url` cədvəli

4\. Cache: Redis-də tez-tez istifadə olunanları saxla

5\. HTTP 301 (daimi) vs 302 (müvəqqəti) yönləndirmə



```

\[Müştəri] → \[Load Balancer] → \[API Server] → \[Redis Cache]

&#x20;                                                   ↓ (miss)

&#x20;                                             \[PostgreSQL DB]

```



</details>



<details>

<summary><b>Sistem dizaynında ən vacib anlayışlar hansılardır?</b></summary>



| Anlayış | Nədir |

|---------|-------|

| \*\*Load Balancer\*\* | Trafiqi serverler arasında böl |

| \*\*CDN\*\* | Statik məzmunu istifadəçiyə yaxın serverden ver |

| \*\*Cache\*\* | Tez-tez istənilən məlumatı sürətli yaddaşda saxla |

| \*\*Database Sharding\*\* | Böyük verilənlər bazasını hissələrə böl |

| \*\*Replication\*\* | Verilənlər bazasını kopyala (master-slave) |

| \*\*Message Queue\*\* | Xidmətlər arasında asinxron mesajlaşma |

| \*\*Microservices\*\* | Böyük tətbiqi kiçik müstəqil xidmətlərə böl |

| \*\*API Gateway\*\* | Bütün API çağrıları üçün tək giriş nöqtəsi |

| \*\*Rate Limiting\*\* | Saniyədə maksimum sorğu sayını məhdudlaşdır |

| \*\*CAP Teoremi\*\* | Consistency, Availability, Partition Tolerance |



</details>



\---



\## 👔 Davranış Sualları (Behavioral)



Bu suallar üçün \*\*STAR metodundan\*\* istifadə et:

\- \*\*S\*\*ituation — Hansı kontekst/vəziyyət idi?

\- \*\*T\*\*ask — Sənin roluun nə idi?

\- \*\*A\*\*ction — Nə etdin?

\- \*\*R\*\*esult — Nəticə nə oldu?



<details>

<summary><b>Özünü tanıt</b></summary>



\*\*Tövsiyə olunan struktur (2 dəqiqə):\*\*

1\. Hazırda kim olduğun (1-2 cümlə)

2\. Ən güclü texniki bacarıqların + bir nəticə (1-2 cümlə)

3\. Niyə bu vəzifəyə müraciət etdin (1 cümlə)



\*\*Nümunə:\*\*

> "Mən 2 ildir React və Node.js ilə full-stack veb tətbiqləri quran bir proqramçıyam. Son layihəmdə e-ticarət platforması üçün tam CRUD API qurdum, Stripe ilə ödəniş inteqrasiyası tamamladım və tətbiqi AWS-də deploy etdim. Bu vəzifəyə müraciət etdim çünkü şirkətin müştəriyönümlü məhsulları və React ekosistemindən istifadəsi mənə çox uyğundur."



</details>



<details>

<summary><b>Ən böyük zəif cəhətin nədir?</b></summary>



\*\*Nə etmə:\*\* "Çox çalışıram" kimi saxta cavab vermə — işəgötürən bilir.



\*\*Nə et:\*\* Real bir zəif cəhəti söylə + üzərindən işlədiyini göstər.



\*\*Nümunə:\*\*

> "Sistem dizaynı (scalability) mövzusunda daha çox inkişaf etməliyəm. Hazırda hər həftə 'System Design Primer' oxuyuram və Kubernetes-ə dair praktiki məşqlər edirəm. Bu sahəni 6 ayda möhkəmləndirməyi hədəfləyirəm."



</details>



<details>

<summary><b>Çətin bir texniki problemlə necə başa çıxdın?</b></summary>



\*\*STAR ilə cavabla:\*\*

\- S: "Layihəmizdə production-da rast gəlinəcəyi gözlənilməyən bir performans problemi yarandı"

\- T: "Problemi tapıb həll etmək mənim vəzifəm idi"

\- A: "Profiling alətləri ilə darboğazı tapdım (N+1 sorğu problemi), eager loading tətbiq etdim"

\- R: "Sorğu sayı 50-dən 3-ə düşdü, page load 3.2s-dən 0.4s-ə endirdi"



</details>



\---



\## 📋 Müsahib Hazırlıq Yol Xəritəsi



\### Junior Müsahib (0-2 il)

\- \[ ] LeetCode Easy-Medium: 50-75 problem

\- \[ ] NeetCode 150-nin ilk 3 kateqoriyası (Arrays, Two Pointers, Sliding Window)

\- \[ ] Seçdiyiniz dilin əsas konsepsiyaları (JS/Python/Java)

\- \[ ] STAR metodu ilə 5 davranış sualı hazırla

\- \[ ] CV-ni nəzərdən keçir, GitHub-u yenilə



\### Mid/Senior Müsahib (2+ il)

\- \[ ] LeetCode Medium-Hard: 100+ problem

\- \[ ] Sistem Dizaynı: URL shortener, Chat sistemi, Instagram kimi məşqlər

\- \[ ] \[System Design Primer](https://github.com/donnemartin/system-design-primer) oxu

\- \[ ] Keçmiş layihələrdəki texniki qərarları izah etməyə hazır ol



\---



\## 🔗 Faydalı Qaynaqlar



\- \[NeetCode.io](https://neetcode.io) — LeetCode problemi + video həll ⭐

\- \[Pramp](https://pramp.com) — Canlı mock müsahib (pulsuz)

\- \[Tech Interview Handbook](https://github.com/yangshun/tech-interview-handbook) — Tam rehber ⭐

\- \[interviewing.io](https://interviewing.io) — Anonim mock müsahib

\- \[Glassdoor](https://glassdoor.com) — Şirkət müsahib sualları



\---



> 📅 Son yenilənmə: Fevral 2026

