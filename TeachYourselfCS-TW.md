# 自學計算機科學

> 本文檔是對 [TeachYourselfCS](https://teachyourselfcs.com) 內容的繁體中文翻譯，原作者為 [Ozan Onay](https://twitter.com/oznova_) 和 [Myles Byrne](https://twitter.com/quackingduck)。如需了解翻譯相關信息或幫助改進翻譯，請參見 [本文檔結尾](#這份指引是誰翻譯的)。
>
> This document is a Taiwan Mardarin version of [TeachYourselfCS](https://teachyourselfcs.com), which is written by [Ozan Onay](https://twitter.com/oznova_) and [Myles Byrne](https://twitter.com/quackingduck). For more information about this translation, please refer to [the end of this document](#這份指引是誰翻譯的).

如果你是一個自學成才的工程師，或者從編程培訓班畢業，那麽你很有必要學習計算機科學。幸運的是，不必為此花上數年光陰和不菲費用去攻讀一個學位：僅僅依靠自己，你就可以獲得世界一流水平的教育💸。

互聯網上，到處都有許多的學習資源，然而精華與糟粕並存。你所需要的，不是一個諸如「200+ 免費在線課程」的清單，而是以下問題的答案：

* 你應當學習 **哪些科目**，為什麽？
* 對於這些科目，**最好的書籍或者視頻課程** 是什麽？

在這份指引中，我們嘗試對這些問題做出確定的回答。

## 簡而言之

大致按照列出的順序，借助我們所建議的教材或者視頻課程（但是最好二者兼用），學習如下的九門科目。目標是先花 100 到 200 個小時學習完每一個科目，然後在你職業生涯中，不時溫習其中的精髓🚀。

| 科目 | 為何要學？ | 最佳書籍 | 最佳視頻 |
|-|-|-|-|
| [編程](#編程) | 不要做一個「永遠沒徹底搞懂」諸如遞歸等概念的程序員。 | [《計算機程序的構造和解釋》](https://book.douban.com/subject/1148282/) | Brian Harvey’s Berkeley CS 61A |
| [計算機系統結構](#計算機系統結構) | 如果你對於計算機如何工作沒有具體的概念，那麽你所做出的所有高級抽象都是空中樓閣。 | [《深入理解計算機系統》](https://book.douban.com/subject/26912767/) | Berkeley CS 61C |
| [算法與數據結構](#算法和數據結構) | 如果你不懂得如何使用棧、隊列、樹、圖等常見數據結構，遇到有難度的問題時，你將束手無策。 | [《算法設計手冊》](https://book.douban.com/subject/4048566/) | Steven Skiena’s lectures |
| [數學知識](#數學知識) | 計算機科學基本上是應用數學的一個「跑偏的」分支，因此學習數學將會給你帶來競爭優勢。 | [《計算機科學中的數學》](https://book.douban.com/subject/33396340/) | Tom Leighton’s MIT 6.042J |
| [操作系統](#操作系統) | 你所寫的代碼，基本上都由操作系統來運行，因此你應當了解其運作的原理。 | [《操作系統導論》](https://book.douban.com/subject/33463930/) | Berkeley CS 162 |
| [計算機網絡](#計算機網絡) | 互聯網已然勢不可擋：理解工作原理才能解鎖全部潛力。 | [《計算機網絡：自頂向下方法》](https://book.douban.com/subject/30280001/) | Stanford CS 144 |
| [數據庫](#數據庫) | 對於多數重要程序，數據是其核心，然而很少人理解數據庫系統的工作原理。 | *[Readings in Database Systems](https://book.douban.com/subject/2256069/)* （暫無中譯本） | Joe Hellerstein’s Berkeley CS 186 |
| [編程語言與編譯器](#編程語言與編譯器) | 若你懂得編程語言和編譯器如何工作，你就能寫出更好的代碼，更輕松地學習新的編程語言。 | *[Crafting Interpreters](https://craftinginterpreters.com/)* | Alex Aiken’s course on Lagunita   |
| [分布式系統](#分布式系統) | 如今，**多數** 系統都是分布式的。 | [《數據密集型應用系統設計》](https://book.douban.com/subject/30329536/) | MIT 6.824 |

## 還是太多？

如果花幾年時間自學 9 門科目讓人望而卻步，我們建議你只專注於兩本書：**《深入理解計算機系統》** 和 **《數據密集型應用系統設計》**。根據我們的經驗，投入到這兩本書的時間可以獲得極高的回報率，特別適合從事網絡應用開發的自學工程師。這兩本書也可以作為上面表格中其他科目的綱領。

## 為什麽要學習計算機科學？

軟件工程師分為兩種：一種充分理解了計算機科學，從而有能力應對充滿挑戰的創造性工作；另一種僅僅憑著對一些高級工具的熟悉而勉強應付。

這兩種人都自稱軟件工程師，都能在職業生涯早期掙到差不多的工資。然而，隨著時間流逝，第一種工程師不斷成長，所做的事情將會越來越有意義且更為高薪，不論是有價值的商業工作、突破性的開源項目、技術上的領導力或者高質量的個人貢獻。

> 全球短信系統每日收發約 200 億條信息，而僅僅靠 57 名工程師，現在的 WhatsApp 每日收發 420 億條。
>
> — Benedict Evans (@BenedictEvans) [2016 年 2 月 2 日](https://twitter.com/BenedictEvans/status/694342874729545729)

第一種工程師總是尋求深入學習計算機科學的方法，或是通過傳統的方法學習，或是在職業生涯中永無止息地學習；第二種工程師
通常浮於表面，只學習某些特定的工具和技術，而不研究其底層的基本原理，僅僅在技術潮流的風向改變時學習新的技能。

如今，湧入計算機行業的人數激增，然而計算機專業的畢業生數量基本上未曾改變。第二種工程師的供過於求正在開始減少他們的工作機會，使他們無法涉足行業內更加有意義的工作。對你而言，不論正在努力成為第一種工程師，還是只想讓自己的職業生涯更加安全，學習計算機科學是唯一可靠的途徑。

> 23333 然而他們……[pic.twitter.com/XVNYlXAHar](https://web.archive.org/web/20170528095858/https://twitter.com/jenna/status/838161631662092289)
>
> — Jenna Bilotta (@jenna) [2017 年 3 月 4 日](https://web.archive.org/web/20170528095858/https://twitter.com/jenna/status/838161631662092289)

## 分科目指引

### 編程

大多數計算機專業本科教學以程序設計「導論」作為開始。這類課程的最佳版本不僅能滿足初學者的需要，還適用於那些在初學編程階段遺漏了某些有益的概念和程序設計模式的人。

對於這部分內容，我們的標準推薦是這部經典著作：[《計算機程序的構造和解釋》](https://book.douban.com/subject/1148282/)。在網絡上，這本書既可供 [免費閱讀（英文版）](https://mitpress.mit.edu/sites/default/files/sicp/full-text/book/book.html)，也作為 [MIT 的免費視頻課程](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-001-structure-and-interpretation-of-computer-programs-spring-2005/video-lectures/)。不過盡管這些視頻課程很不錯，我們對於視頻課程的推薦實際上是 [Brian Harvey 開設的 SICP 課程](https://archive.org/details/ucberkeley-webcast-PL3E89002AA9B9879E?sort=titleSorter)（即 Berkeley 的 61A 課程）。比起 MIT 的課程，它更加完善，更適用於初學者。

我們建議至少學完 SICP 的前三章，並完成配套的習題。如果需要額外的練習，可以去解決一些小的程序設計問題，比如 [exercism](http://exercism.io)。

> **中文翻譯新增：**
>
> * 關於 SICP 國內視頻觀看地址
>   * [MIT 的免費視頻課程（中英字幕）](https://www.bilibili.com/video/av8515129/)
>   * [Brian Harvey 開設的 SICP 課程（英文字幕）](https://www.bilibili.com/video/av40460492/)
> * Scheme 學習的相關資源參見：<https://github.com/DeathKing/Learning-SICP>
> * 更詳細的補充說明：[#3](https://github.com/izackwu/TeachYourselfCS-CN/issues/3)

自從 2016 年首次發布這份指南以來，最常被問到的一個問題是，我們是否推薦由 John DeNero 講授的更新的 CS 61A 課程，以及配套的書籍 [*Composing Programs*](https://composingprograms.com/)，這本書「繼承自 SICP」 但使用 Python 講解。我們認為 DeNero 的課程也很不錯，有的學生可能更喜歡，但我們還是建議把 SICP、Scheme 和 Brian Harvey 的視頻課程作為首選。

為什麽這麽說呢？因為 SICP 是獨一無二的，它可以——至少很有可能——改變你對計算機和編程的基本認識。不是每個人都有這樣的體驗。有的人討厭這本書，有的人看了前幾頁就放棄了。但潛在的回報讓它值得一讀。

如果你覺得 SICP 過於難，試試 *Composing Programs*。如果還是不合適，那我們推薦 《程序設計方法》（[中文版](https://book.douban.com/subject/1140942/)，[英文版](http://www.htdp.org/)） ；如果你覺得 SICP 過於簡單，那我們推薦 [*Concepts, Techniques, and Models of Computer Programming*](https://book.douban.com/subject/1782316/)。如果讀這些書讓你覺得沒有收獲，也許你應該先學習其他科目，一兩年後再重新審視編程的理念。

> 新版原文刪除了對 *Concepts, Techniques, and Models of Computer Programming* 一書的推薦，但這本書對各種編程模型有深入的見解，值得一讀。所以譯文中依然保留。
> — 譯者注

最後，有一點要說明的是：本指南 **不適用** 於完全不懂編程的新手。我們假定你是一個沒有計算機專業背景的程序員，希望填補一些知識空白。事實上，我們把「編程」章節包括進來只是提醒你還有更多知識需要學習。對於那些從來沒有學過編程，但又想學的人來說，這份 [指南](https://www.reddit.com/r/learnprogramming/wiki/faq#wiki_getting_started) 更合適。

[![計算機程序的構造和解釋](https://user-images.githubusercontent.com/20233656/66758473-ef7bff80-eed0-11e9-944a-15ae5c8542ca.jpg)](https://book.douban.com/subject/1148282/)

### 計算機系統結構

計算機系統結構——有時候又被稱為「計算機系統」或者「計算機組成」——是了解軟件底層的的重要視角。根據我們的經驗，這是自學的軟件工程師最容易忽視的領域。

我們最喜歡的入門書是 [《深入理解計算機系統》](https://book.douban.com/subject/26912767/)。典型的 [計算機體系結構導論課程](http://csapp.cs.cmu.edu/3e/courses.html) 會涵蓋本書的 1-6 章。

我們喜愛《深入理解計算機系統》，因為它的實用性，並且站在程序員的視角。雖然計算機體系結構的內容比本書所涉及的內容多得多，但對於那些想了解計算機系統以求編寫更快、更高效、更可靠的軟件的人來說，這本書是很好的起點。

對於那些既想了解這個主題又想兼顧硬件和軟件的知識的人來說，我們推薦 [《計算機系統要素》](https://book.douban.com/subject/1998341/)，又名「從與非門到俄羅斯方塊」（Nand2Tetris），這本書規模宏大，讓讀者對計算機內的所有部分如何協同工作有完全的認識。這本書的每一章節對應如何構建計算機整體系統中的一小部分，從用 HDL（硬件描述語言）寫基本的邏輯門電路出發，途經 CPU 和匯編，最終抵達諸如俄羅斯方塊這般規模的應用程序。

我們推薦把此書的前六章讀完，並完成對應的項目練習。這麽做，你將更加深入地理解，計算機體系結構和運行其上的軟件之間的關系。

這本書的前半部分（包括所有對應的項目）均可從 [Nand2Tetris 的網站上](http://www.nand2tetris.org) 免費獲得。同時，在 Coursera 上，這是一門 [視頻課程](https://www.coursera.org/learn/build-a-computer)。

為了追求簡潔和緊湊，這本書犧牲了內容上的深度。尤其值得注意的是，流水線和存儲層次結構是現代計算機體系結構中極其重要的兩個概念，然而這本書對此幾乎毫無涉及。

當你掌握了 Nand2Tetris 的內容後，我們推薦要麽回到《深入理解計算機系統》，或者考慮 Patterson 和 Hennessy 二人所著的 [《計算機組成與設計》](https://book.douban.com/subject/26604008/)，一本優秀的經典著作。這本書中的不同章節重要程度不一，因此我們建議根據 Berkeley 的 [CS61C 課程](http://inst.eecs.berkeley.edu/~cs61c/sp15/) 「計算機體系結構中的偉大思想」來著重閱讀一些章節。這門課的筆記和實驗在網絡上可以免費獲得，並且在 [互聯網檔案](https://archive.org/details/ucberkeley-webcast-PL-XXv-cvA_iCl2-D-FS5mk0jFF6cYSJs_) 中有這門課程的過往資料。

[![深入理解計算機系統](https://user-images.githubusercontent.com/20510068/82109944-12270d00-976d-11ea-85a9-774e4f762ec9.png)](https://book.douban.com/subject/26912767/) [![計算機系統要素](https://user-images.githubusercontent.com/20233656/66758695-60231c00-eed1-11e9-8422-a4acfb10a390.jpg)](http://www.nand2tetris.org)

> 硬件是平台。
>
> — Mike Acton, Engine Director at Insomniac Games
> （[觀看他在 CppCon 上的演說](https://www.youtube.com/watch?v=rX0ItVEVjHc)）

### 算法與數據結構

正如幾十年來的共識，我們認為，計算機科學教育所賦予人們的最大能量在於對常見算法和數據結構的熟悉。此外，這也可以訓練一個人對於各種問題的解決能力，有助於其他領域的學習。

關於算法與數據結構，有成百上千的書可供使用，但是我們的最愛是 Steven Skiena 編寫的 [《算法設計手冊》](https://book.douban.com/subject/4048566/) 。顯而易見，他對此充滿熱愛，迫不及待地想要幫助其他人理解。在我們看來，這本書給人一種煥然一新的體驗，完全不同於那些更加經常被推薦的書（比如 Cormen、Leiserson、Rivest、Stein 或 Sedgewick 的書，後兩者充斥著過多的證明，不適合以 **解決問題** 為導向的學習）。

如果你更喜歡視頻課程，[Skiena 慷慨地提供了他的課程](https://www.youtube.com/watch?v=A2bFN3MyNDA&list=PLOtl7M3yp-DX32N0fVIyvn7ipWKNGmwpp)。此外，Tim Roughgarden 的課程也很不錯，
在 Stanford 的 MOOC 平台 Lagunita，或者 [Coursera](https://www.coursera.org/specializations/algorithms) 上均可獲得。Skiena 和 Roughgarden 的這兩門課程沒有優劣之分，選擇何者取決於個人品味。

至於練習，我們推薦學生在 [Leetcode](https://leetcode.com) 上解決問題。Leetcode 上的問題往往有趣且帶有良好的解法和討論。此外，在競爭日益激烈的軟件行業，這些問題可以幫助你評估自己應對技術面試中常見問題的能力。我們建議解決大約 100 道隨機挑選的 Leetcode 問題，作為學習的一部分。

最後，我們強烈推薦 [《怎樣解題》](https://book.douban.com/subject/2124114/)。這本書極為優秀且獨特，指導人們解決廣義上的問題，因而一如其適用於數學，它適用於計算機科學。

[![算法設計手冊](https://user-images.githubusercontent.com/20233656/66759121-361e2980-eed2-11e9-913c-8fc48c67122a.jpg)](https://book.douban.com/subject/4048566/) [![怎樣解題](https://user-images.githubusercontent.com/20233656/66759282-8e552b80-eed2-11e9-89de-16b1f8d82e78.jpg)](https://book.douban.com/subject/2124114/)

> 我可以廣泛推薦的方法只有一個： 寫之前先思考。
>
>— Richard Hamming

### 數學知識

從某個角度說，計算機科學是應用數學的一個「發育過度」的分支。盡管許多軟件工程師試圖——並且在不同程度上成功做到——忽視這一點，我們鼓勵你用學習來擁抱數學。如若成功，比起那些沒有掌握數學的人，你將獲得巨大的競爭優勢。

對於計算機科學，數學中最相關的領域是「離散數學」，其中的「離散」與「連續」相對立，大致上指的是應用數學中那些有趣的主題，而不是微積分之類的。由於定義比較含糊，試圖掌握離散數學的全部內容是沒有意義的。較為現實的學習目標是，了解邏輯、排列組合、概率論、集合論、圖論以及密碼學相關的一些數論知識。考慮到線性代數在計算機圖形學和機器學習中的重要性，該領域同樣值得學習。

學習離散數學，我們建議從 [László Lovász 的課程筆記](http://www.cs.elte.hu/~lovasz/dmbook.ps) 開始。Lovász 教授成功地讓這些內容淺顯易懂且符合直覺，因此，比起正式的教材，這更適合初學者。

對於更加高階的學習，我們推薦 [《計算機科學中的數學》](https://book.douban.com/subject/33396340/)，MIT 同名課程的課程筆記，篇幅與書籍相當（事實上，現已出版）。這門課程的視頻同樣 [可免費獲得](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-042j-mathematics-for-computer-science-fall-2010/video-lectures/)，是我們所推薦的學習視頻。

對於線性代數，我們建議從 [Essence of linear algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab) 系列視頻開始，然後再去學習 Gilbert Strang 的 [《線性代數導論》](https://book.douban.com/subject/34820335/) 和 [視頻課程](https://ocw.mit.edu/courses/mathematics/18-06-linear-algebra-spring-2010/video-lectures/)。

[![計算機科學中的數學](https://user-images.githubusercontent.com/20233656/66759673-4387e380-eed3-11e9-8469-3e677d108e91.jpg)](https://book.douban.com/subject/33396340/)

> 如果人們不相信數學是簡單的，那麽只能是因為他們沒有意識到生活有多麽覆雜。
>
>— John von Neumann

### 操作系統

[《操作系統概念》](https://book.douban.com/subject/30297919/)（「恐龍書」）和 [《現代操作系統》](https://book.douban.com/subject/27096665/) 是操作系統領域的經典書籍。二者都因為寫作風格和對學生不友好而招致了一些批評。

[《操作系統導論》（*Operating Systems: Three Easy Pieces*）](https://book.douban.com/subject/33463930/) 是一個不錯的替代品，並且 [可在網上免費獲得（英文版）](http://pages.cs.wisc.edu/~remzi/OSTEP/)。我們格外喜歡這本書的結構，並且認為這本書的習題很值得一做。

在讀完《操作系統導論》後，我們鼓勵你探索特定操作系統的設計。可以借助「{OS name} Internals」風格的書籍，比如 [*Lion's commentary on Unix*](https://www.amazon.com/Lions-Commentary-Unix-John/dp/1573980137/)， [*The Design and Implementation of the FreeBSD Operating System*](https://www.amazon.com/Design-Implementation-FreeBSD-Operating-System/dp/0321968972/)，以及 [*Mac OS X Internals*](https://www.amazon.com/Mac-OS-Internals-Systems-Approach/dp/0321278542/)。對於 Linux ，我們推薦 Robert Love 的 [《Linux 內核設計與實現》](https://book.douban.com/subject/6097773/)。

為了鞏固對操作系統的理解，閱讀小型系統內核的代碼並且為其增加特性是一個很不錯的方法。比如，[xv6](https://pdos.csail.mit.edu/6.828/2016/xv6.html)，由 MIT 的一門課程所維護的從 Unix V6 到 ANSI C 和 x86 的移植，就是一個很棒的選擇。《操作系統導論》有一個附錄，記載了一些可能的 [xv6 實驗項目](http://pages.cs.wisc.edu/~remzi/OSTEP/lab-projects-xv6.pdf)，其中充滿了關於潛在項目的很棒想法。

[![操作系統導論](https://user-images.githubusercontent.com/20233656/66759780-78943600-eed3-11e9-8eb5-6472c318c265.jpg)](https://book.douban.com/subject/33463930/)

### 計算機網絡

鑒於有那麽多關於網絡服務端和客戶端的軟件工程，計算機網絡是計算機科學中價值最為「立竿見影」的領域之一。我們的學生，系統性地學習了計算機網絡，最終能夠理解那些曾困擾他們多年的術語、概念和協議。

在這一主題上，我們最愛的書籍是 [《計算機網絡：自頂向下方法》](https://book.douban.com/subject/30280001/)。書中的小項目和習題相當值得練習，尤其是其中的「Wireshark labs」（[這部分在網上可以獲得](http://www-net.cs.umass.edu/wireshark-labs/)）。

如果更喜歡視頻課程，我們推薦 Stanford 的 [*Introduction to Computer Networking*](https://lagunita.stanford.edu/courses/Engineering/Networking-SP/SelfPaced/about)，可在他們的 MOOC 平台 Lagunita 上免費觀看。

對於計算機網絡的學習，做項目比完成小的習題更有益。一些可能的項目有：HTTP 服務器，基於 UDP 的聊天 APP，[迷你 TCP 棧](http://jvns.ca/blog/2014/08/12/what-happens-if-you-write-a-tcp-stack-in-python/)，代理，負載均衡器，或者分布式哈希表。

[![《計算機網絡：自頂向下方法》](https://user-images.githubusercontent.com/20233656/66760004-d9bc0980-eed3-11e9-9b3f-74bf54b9571f.jpg)](https://book.douban.com/subject/30280001/)

> 你無法盯著水晶球預見未來，未來的互聯網何去何從取決於社會。
>
>— Bob Kahn

### 數據庫

比起其他主題，自學數據庫系統需要更多的付出。這是一個相對年輕的研究領域，並且出於很強的商業動機，研究者把想法藏在緊閉的門後。此外，許多原本有潛力寫出優秀教材的作者反而選擇了加入或創立公司。

鑒於如上情況，我們鼓勵自學者大體上拋棄教材，而是從 [2015 年春季學期的 CS 186 課程](https://archive.org/details/UCBerkeley_Course_Computer_Science_186)（Joe Hellerstein 在 Berkeley 的數據庫課程）開始，然後前往閱讀論文。

對於初學者，有一篇格外值得提及的論文：[*Architecture of a Database System*](http://db.cs.berkeley.edu/papers/fntdb07-architecture.pdf)。這篇論文提供了獨特的對關系型數據庫管理系統（RDBMS）如何工作的高層次觀點，是後續學習的實用梗概。

[*Readings in Database Systems*](https://book.douban.com/subject/2256069/)，或者以 [數據庫「紅書」](http://www.redbook.io/) 更為人知，是由 Peter Bailis、Joe Hellerstein 和 Michael Stonebraker 編纂的論文合集。對於那些想要在 CS 186 課程的水平更進一步的學習者，「紅書」應當是下一步。

如果你堅持一定要一本導論教材，那我們推薦 Ramakrishnan 和 Gehrke 所著的 [《數據庫管理系統：原理與設計》](https://book.douban.com/subject/1155934/)。如需更深一步，Jim Gray 的經典著作 [*Transaction Processing: Concepts and Techniques*](https://book.douban.com/subject/2586390/) 值得一讀，不過我們不建議把這本書當作首要資源。

如果沒有編寫足夠數量的代碼，很難鞏固數據庫理論。CS 186 課程的學生給 Spark 添加特性，倒是不錯的項目，不過我們僅僅建議從零實現一個簡單的關系型數據庫管理系統。自然，它將不會有太多的特性，但是即便只實現典型的關系型數據庫管理系統每個方面最基礎的功能，也是相當有啟發的。

最後，數據模型往往是數據庫中一個被忽視的、教學不充分的方面。關於這個主題，我們推薦的書籍是 [*Data and Reality: A Timeless Perspective on Perceiving and Managing Information in Our Imprecise World*](https://book.douban.com/subject/17915870/)。

[![Readings in Database Systems](https://user-images.githubusercontent.com/20233656/66760126-08d27b00-eed4-11e9-82c6-46c571036aa1.jpg)](https://book.douban.com/subject/2256069/) [![數據庫管理系統：原理與設計](https://user-images.githubusercontent.com/20233656/66760358-85655980-eed4-11e9-9130-66d2ecea5700.jpg)](https://book.douban.com/subject/1155934/)

### 編程語言與編譯器

多數程序員學習編程語言的知識，而多數計算機科學家學習編程語言 **相關** 的知識。這使得計算機科學家比起程序員擁有顯著的優勢，即便在編程領域！因為他們的知識可以推而廣之：相較只學習過特定編程語言的人，他們可以更深入更快速地理解新的編程語言。

我們推薦的入門書是 Bob Nystrom 所著的優秀的 [*Crafting Interpreters*](https://craftinginterpreters.com/contents.html)，可在網上免費獲取。這本書條理清晰，富有趣味性，非常適合那些想要更好地理解語言和語言工具的人。我們建議你花時間讀完整本書，並嘗試任何一個感興趣的「挑戰」。

另一本更為傳統的推薦書籍是 [《編譯原理》](https://book.douban.com/subject/3296317/)，通常稱為「龍書」。不幸的是，這本書不是為自學者而設計的，而是供教師從中挑選一些主題用於 1-2 學期的教學。

如果你選擇使用龍書進行自學，你需要從中甄選主題，而且最好是在導師的幫助下。我們建議依據某個視頻課程來設定學習的結構，然後按需從龍書中獲取深入的內容。我們推薦的在線課程是 [Alex Aiken 在 MOOC 平台 edX 所開設的](https://www.edx.org/course/compilers)。

[![編譯原理](https://user-images.githubusercontent.com/20233656/66760486-ca898b80-eed4-11e9-80ba-df298ac8d5da.jpg)](https://book.douban.com/subject/3296317/)

> 不要做一個只寫樣板代碼的程序員。相反，給用戶和其他程序員創造工具。從紡織工業和鋼鐵工業中學習歷史教訓：你想制造機器和工具，還是操作這些機器？
>
>— Ras Bodik 在他的編譯器課程伊始

### 分布式系統

隨著計算機在數量上的增加，計算機同樣開始 **分散**。盡管商業公司過去願意購買越來越大的大型機，現在的典型情況是，甚至很小的應用程序都同時在多台機器上運行。思考這樣做的利弊權衡，即是分布式系統的研究所在，也是越來越重要的一項技能。

我們推薦的自學參考書是 Martin Kleppmann 的 [《數據密集型應用系統設計》](https://book.douban.com/subject/30329536/)。與傳統的教科書相比，它是一本為實踐者設計的具有很高的可讀性的書，並且保持了深度和嚴謹性。

對於那些偏愛傳統教材，或者希望可以從網上免費獲取的人，我們推薦的教材是 Maarten van Steen 和 Andrew Tanenbaum 所著的 《分布式系統原理與範型》（[中文第二版](https://book.douban.com/subject/3108801/)，[英文第三版](https://book.douban.com/subject/26979326/)）。

對於喜歡視頻課程的人，[MIT 的 6.824](https://www.youtube.com/watch?v=cQP8WApzIQQ&list=PLrw6a1wE39_tb2fErI4-WkMbsvGQk9_UB) 是一門很好的在線視頻課程，由 Robert Morris 教授的研究生課程，在 [這里](https://pdos.csail.mit.edu/6.824/schedule.html) 可以看到課程安排。

不管選擇怎樣的教材或者其他輔助資料，學習分布式系統必然要求閱讀論文。[這里](http://dsrg.pdos.csail.mit.edu/papers/) 有一個不錯的論文清單，而且我們強烈建議你出席你當地的 [Papers We Love](http://paperswelove.org/)（僅限美國）。

[![數據密集型應用系統設計](https://user-images.githubusercontent.com/20510068/82111034-94ff9600-9774-11ea-9d49-90b00f746659.png)](https://book.douban.com/subject/30329536/)

## 常見問題解答

### 這份指引的目標受眾是？

我們面向自學的軟件工程師、培訓班學生、「早熟的」高中生或者想要通過自學補充正式教育的大學生。關於何時開啟這段自學旅程，完全取決於個人，不過多數人在有一定的職業經歷後深入學習計算機科學理論會獲益匪淺。比如，我們注意到，如果學生在工作中曾經使用過數據庫，他們會 **喜愛** 學習數據庫系統課程；如果學生從事過一兩個 Web 項目，他們會 **喜愛** 學習計算機網絡。

### 人工智能/計算機圖形學/XX 主題怎麽樣？

我們試圖把計算機科學主題清單限制到那些我們認為 **每一個軟件工程師** 都應該了解的內容，不限於專業或行業。擁有了這些基礎，你將能更加輕松地挑選教材或論文，然而無需指引地學習核心概念。在這里，我們給出一些其他常見主題的自學起點：

* 人工智能：通過觀看視頻並完成 Pacman 項目來學習 [Berkeley 的 AI 課程](http://ai.berkeley.edu/)。至於教材，使用 Russell 和 Norvig 編寫的 [《人工智能：一種現代方法》](https://book.douban.com/subject/25796281/)。
* 機器學習：學習吳恩達在 Coursera 上的課程。耐心學習，先確保理解了基礎概念再奔向類如深度學習的誘人新主題。
* 計算機圖形學：學習 [Berkeley CS 184 課程](http://inst.eecs.berkeley.edu/~cs184/fa12/onlinelectures.html) 的材料，使用 [《計算機圖形學：原理及實踐》](https://book.douban.com/subject/30402778/) 作為教材。

### 一定要嚴格遵守推薦的學習次序嗎？

事實上，所有主題之間都有一定程度的重疊，彼此循環引用。以離散數學和算法的關系為例：先學習數學可以幫助你更深入地分析和理解算法，然而先學習算法可以為學習離散數學提供更大的動力和應用背景。理想情況下，你將在你的職業生涯多次重溫二者。

因此，我們所推薦的次序主要是為了幫助你 **起步**……如果你出於某種強烈的原因而傾向以不同的順序學習，那也沒有關系，勇敢開始吧！不過在我們看來，最重要的「先決條件」是：先學計算機體系結構再學操作系統或數據庫，先學計算機網絡和操作系統再學分布式系統。

### 和 Open Source Society、freeCodeCamp curricula 等比起來，這份指引？

[OSS 指引](https://github.com/open-source-society/computer-science) 涵蓋太多主題，在許多主題中推薦劣質資源，沒有就特定課程哪些方面有價值提供原因或指引。我們努力對這份指引中的課程加以限制，僅僅包括那些你作為軟件工程師 **確實需要了解的**，不論你的專業方向，並且對每門課程為何必要做出了解釋以幫助你理解。

FreeCodeCamp 主要關注編程，而不是計算機科學。至於你為什麽要學習計算機科學，參見 [上文](#為什麽要學習計算機科學)。如果你是個新手，我們建議先學 freeCodeCamp 的課程，一兩年後再回歸本指南。

### XX 編程語言怎麽樣？

學習一門特定的編程語言和學習計算機科學的一個領域完全不在一個維度——相比之下，學習語言 **容易** 且 **缺乏價值**。如果你已經了解了一些語言，我們強烈建議遵照我們的指引，然後在學習的空當中習得語言，或者暫且不管以後再說。如果你已經把編程學得不錯了（比如學完了 **《計算機程序的構造和解釋》**），尤其是如果你學習過編譯器，那麽面對一門新的語言，你只需要花一個周末稍多的時間即可基本掌握，之後你可以在工作中學習相關的類庫/工具/生態。

### XX 流行技術怎麽樣？

沒有任何一種技術的重要程度可以達到學習其使用足以成為計算機科學教學的核心部分。不過，你對學習那門技術充滿熱情，這很不錯。訣竅是先從特定的技術回退到基本的領域或概念，判斷這門流行技術在技術的宏觀大局中位於何處，然後才深入學習這門技術。

### 為什麽你們還在推薦 SICP?

先嘗試讀一下，有些人覺得 SICP 讓人神魂顛倒，這在其他書很少見。如果你不喜歡，你可以嘗試其他的東西，也許以後再回到 SICP。

### 為什麽你們還在推薦龍書？

龍書依舊是內容最為完整的編譯器單本書籍。由於過分強調一些如今不夠時新的主題的細節，比如解析，這本書招致了惡評。然而事實上，這本書從未打算供人一頁一頁的學習，而僅僅是為了給教師準備一門課程提供足夠的材料。類似地，自學者可以從書中量身按需挑選主題，或者最好依照公開課授課教師在課程大綱中的建議。

### 如何便宜獲取教材？

我們所建議的許多教材在網上都可以免費獲得，這多虧了作者們的慷慨。對於那些不免費的書籍，我們建議購買舊版本的二手書籍。廣而言之，如果一本教材有多個版本，舊版本大概率是完全足夠使用的。即便新版本的價格是舊版本的 10 倍，新版本也絕不可能比舊版本好 10 倍！

**中文翻譯新增：** 事實上，比起美國，在國內購買技術書籍可以說是相當「廉價」了。如果仍舊尋求更加便宜的購買渠道，可以參考這篇 V2EX 上的 [討論帖子](https://www.v2ex.com/t/578615)，其中提到了一些不錯的購買渠道。

### 這份指引是誰寫的？

這份指引由 [Bradfield School of Computer Science](https://bradfieldcs.com)（舊金山）的兩位教員：[Ozan Onay](https://twitter.com/oznova_) 和 [Myles Byrne](https://twitter.com/quackingduck) 編寫，並由 Oz 於 2020 年更新。這份指引基於我們對數千名自學成才的工程師和培訓班學生教授計算機科學基礎的經驗。感謝我們所有學生對自學資源的持續反饋。

只要有足夠的時間和動力，我們非常有信心，你可以自學完以上所有課程。如果你喜歡一個集中式、結構化、由教師指導的課程，你可能對我們的 [計算機科學強化班](https://bradfieldcs.com/csi/) 感興趣。我們 [不建議](https://ozwrites.com/masters/) 你去攻讀碩士學位。

### 這份指引是誰翻譯的？

這份指引的中文翻譯是 [社區共同貢獻的成果](https://github.com/izackwu/TeachYourselfCS-CN/)，我們歡迎任何反饋和改進！
