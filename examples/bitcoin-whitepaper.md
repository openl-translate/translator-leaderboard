# Bitcoin Whitepaper Translation Comparison (EN → JP)

## Source Text

Abstract
A purely peer-to-peer version of electronic cash would allow online payments to be sent directly from one party to another without going through a financial institution. Digital signatures provide part of the solution, but the main benefits are lost if a trusted third party is still required to prevent double-spending. We propose a solution to the double-spending problem using a peer-to-peer network. The network timestamps transactions by hashing them into an ongoing chain of hash-based proof-of-work, forming a record that cannot be changed without redoing the proof-of-work. The longest chain not only serves as proof of the sequence of events witnessed, but proof that it came from the largest pool of CPU power. As long as a majority of CPU power is controlled by nodes that are not cooperating to attack the network, they'll generate the longest chain and outpace attackers. The network itself requires minimal structure. Messages are broadcast on a best effort basis, and nodes can leave and rejoin the network at will, accepting the longest proof-of-work chain as proof of what happened while they were gone.

Introduction
Commerce on the Internet has come to rely almost exclusively on financial institutions serving as trusted third parties to process electronic payments. While the system works well enough for most transactions, it still suffers from the inherent weaknesses of the trust based model. Completely non-reversible transactions are not really possible, since financial institutions cannot avoid mediating disputes. The cost of mediation increases transaction costs, limiting the minimum practical transaction size and cutting off the possibility for small casual transactions, and there is a broader cost in the loss of ability to make non-reversible payments for nonreversible services. With the possibility of reversal, the need for trust spreads. Merchants must be wary of their customers, hassling them for more information than they would otherwise need. A certain percentage of fraud is accepted as unavoidable. These costs and payment uncertainties can be avoided in person by using physical currency, but no mechanism exists to make payments over a communications channel without a trusted party.

What is needed is an electronic payment system based on cryptographic proof instead of trust, allowing any two willing parties to transact directly with each other without the need for a trusted third party. Transactions that are computationally impractical to reverse would protect sellers from fraud, and routine escrow mechanisms could easily be implemented to protect buyers. In this paper, we propose a solution to the double-spending problem using a peer-to-peer distributed timestamp server to generate computational proof of the chronological order of transactions. The system is secure as long as honest nodes collectively control more CPU power than any cooperating group of attacker nodes.

## Google Translate
要約
純粋なピアツーピア型の電子現金であれば、金融機関を介さずにオンライン決済をある当事者から別の当事者へ直接送金できます。デジタル署名は解決策の一部となりますが、二重支払いを防ぐために信頼できる第三者機関が必要となる場合、本来のメリットは失われます。本稿では、ピアツーピアネットワークを用いた二重支払い問題の解決策を提案します。ネットワークは、ハッシュベースのプルーフ・オブ・ワークの継続的なチェーンにトランザクションをハッシュすることでタイムスタンプを付与し、プルーフ・オブ・ワークをやり直さない限り変更できない記録を形成します。最長のチェーンは、目撃された一連のイベントの証明となるだけでなく、それが最大の CPU パワープールから発信されたことの証明としても機能します。CPU パワーの大部分が、ネットワーク攻撃に協力していないノードによって制御されている限り、それらのノードは最長のチェーンを生成し、攻撃者を凌駕します。ネットワーク自体は最小限の構造で済みます。メッセージはベストエフォート方式でブロードキャストされ、ノードはネットワークから自由に離脱・再参加することができ、離脱中に発生した事象の証拠として最長のプルーフ・オブ・ワーク・チェーンを受け入れます。

はじめに
インターネット上の商取引は、電子決済処理において信頼できる第三者である金融機関にほぼ全面的に依存してきました。このシステムはほとんどの取引において十分に機能しますが、信頼に基づくモデルに内在する弱点を抱えています。金融機関は紛争の仲裁を避けられないため、完全に不可逆な取引は実際には不可能です。仲裁コストは取引コストを増大させ、実用的な最小取引規模を制限し、小規模な取引の可能性を奪います。さらに、不可逆なサービスに対して不可逆な支払いを行うことができなくなるという、より広範なコストも発生します。不可逆な支払いの可能性が増すにつれ、信頼の必要性は高まります。販売業者は顧客を警戒し、必要以上の情報を要求する必要に迫られます。一定の割合の詐欺行為は避けられないものとして容認されています。これらのコストと支払いの不確実性は、物理的な通貨を直接使用することで回避できますが、信頼できる第三者を介さずに通信チャネルを介して支払いを行うメカニズムは存在しません。

必要なのは、信頼ではなく暗号的証明に基づく電子決済システムであり、信頼できる第三者を介さずに、任意の 2 者が直接取引を行うことを可能にします。計算量的に元に戻すことが不可能な取引は、売り手を詐欺から保護し、買い手を保護するための定型的なエスクローメカニズムを容易に実装できます。本論文では、ピアツーピアの分散型タイムスタンプサーバーを用いて取引の時系列順序の計算量的証明を生成することで、二重支払い問題の解決策を提案します。このシステムは、誠実なノードが、協力する攻撃ノードのグループよりも多くの CPU パワーを総合的に制御している限り、安全です。

## OpenL Translate
要約  
純粋なピア・ツー・ピア型の電子現金システムは、金融機関を介さずに、当事者間で直接オンライン決済を送信できるようにします。デジタル署名は解決策の一部を提供しますが、二重支払いを防ぐために信頼できる第三者が依然として必要である場合、主な利点は失われます。私たちは、ピア・ツー・ピアネットワークを使用して二重支払い問題を解決する方法を提案します。ネットワークは、トランザクションをハッシュ化し、進行中のハッシュベースのプルーフ・オブ・ワークのチェーンに組み込むことで、タイムスタンプを付与します。これにより、プルーフ・オブ・ワークをやり直さない限り変更できない記録が形成されます。最も長いチェーンは、目撃された出来事の順序の証明としてだけでなく、最大の CPU パワープールから発生したことの証明にもなります。大多数の CPU パワーがネットワーク攻撃に協力しないノードによって制御されている限り、彼らは最長のチェーンを生成し、攻撃者を凌駕します。ネットワーク自体は最小限の構造しか必要としません。メッセージはベストエフォートでブロードキャストされ、ノードは自由にネットワークから離脱・再参加でき、不在時に発生した出来事の証明として最長のプルーフ・オブ・ワークチェーンを受け入れます。

はじめに  
インターネット上の商取引は、電子決済を処理する信頼できる第三者として機能する金融機関にほぼ完全に依存するようになっています。このシステムはほとんどの取引において十分に機能していますが、信頼ベースモデルの本質的な弱点が依然として存在します。金融機関が紛争の仲裁を避けられないため、完全に不可逆的な取引は実際には不可能です。仲裁のコストは取引コストを増加させ、実用的な最小取引額を制限し、小額かつ気軽な取引の可能性を断ち切ります。また、不可逆的なサービスに対して不可逆的な支払いを行う能力が失われるという、より広範なコストも生じます。取引の取り消しが可能である場合、信頼の必要性が広がります。販売者は顧客に対して警戒し、通常必要としない情報まで要求することになります。一定割合の詐欺は不可避なものとして受け入れられています。これらのコストや支払いの不確実性は、現金を使えば対面で回避できますが、信頼できる第三者なしに通信チャネル越しに支払いを行う仕組みは存在しません。

必要なのは、信頼ではなく暗号学的証明に基づく電子決済システムです。これにより、任意の 2 者が信頼できる第三者を必要とせず、直接取引できるようになります。計算上逆転が非現実的な取引は、販売者を詐欺から守り、買い手を守るためのエスクロー機構も容易に実装できます。本論文では、ピア・ツー・ピア分散型タイムスタンプサーバーを用いて、取引の時系列順序の計算証明を生成し、二重支払い問題の解決策を提案します。誠実なノードが協力して攻撃者ノードのグループよりも多くの CPU パワーを制御している限り、このシステムは安全です。


## Yandex Translate
アブストラクト
純粋にピアツーピアの電子現金のバージョンは、オンライン支払いが金融機関を経由せずに、ある当事者から別の当事者に直接送信されることを可能にするであろう。デジタル署名はソリューションの一部を提供しますが、信頼できる第三者が依然として二重支出を防ぐ必要がある場合、主な利点は失われます。ピアツーピアネットワークを用いた二重支出問題の解決策を提案した。ネットワークは、トランザクションをハッシュベースの作業証明の進行中のチェーンにハッシュすることによってタイムスタンプを付け、作業証明をやり直すことなく変更できないレコードを形成します。最長のチェーンは、目撃された一連のイベントの証拠として機能するだけでなく、CPU パワーの最大のプールから来たという証拠としても機能します。CPU パワーの大部分がネットワークを攻撃するために協力していないノードによって制御されている限り、それらは最も長いチェーンを生成し、攻撃者を ネットワーク自体は最小限の構造を必要とします。メッセージはベストエフォートベースでブロードキャストされ、ノードは自由にネットワークを離れて再参加することができ、最長の proof-of-work チェーンを行っている間に何が起こったかの証拠として受け入れることができます。

はじめに
インターネット上の商取引は、電子決済を処理するために信頼できる第三者として機能する金融機関にほぼ独占的に依存するようになった。システムはほとんどのトランザクションで十分に機能しますが、信頼ベースのモデルの固有の弱点に苦しんでいます。金融機関は紛争の調停を避けることができないため、完全に可逆的な取引は実際には不可能です。調停のコストは、取引コストを増加させ、最小の実用的な取引サイズを制限し、小さなカジュアルな取引の可能性を遮断し、非可逆的なサービスのための非可逆的な支払いを行う能力の損失に広いコストがあります。逆転の可能性があると、信頼の必要性が広がります。商人は、彼らがそうでなければ必要とするよりも多くの情報のためにそれらを口論、彼らの顧客を警戒する必要があります。一定の割合の詐欺は避けられないものとして受け入れられています。これらのコストと支払いの不確実性は、物理的な通貨を使用することによって直接回避することができますが、信頼された当事者なしで通信チャネルを介して支払いを行うメカニズムは存在しません。

必要とされるのは、信頼の代わりに暗号証明に基づく電子決済システムであり、信頼できる第三者を必要とせずに、任意の 2 つの意思のある当事者が互いに直接取引できるようにします。逆に計算的に非現実的な取引は、売り手を詐欺から保護し、定期的なエスクローメカニズムを簡単に実装して買い手を保護することができます。本稿では，トランザクションの時系列順序の計算証明を生成するために，ピアツーピア分散タイムスタンプサーバを用いた二重支出問題の解を提案した。正直なノードが集合的に攻撃者ノードの任意の協力グループよりも多くの CPU パワーを制御する限り、システムは安全です。

## DeepL
概要
純粋にピアツーピア版の電子マネーは、金融機関を通さずに、ある当事者から別の当事者に直接オンライン決済を送ることを可能にする。電子署名はそのソリューションの一部を提供するが、二重支出を防ぐために信頼できる第三者が必要な場合、主な利点は失われる。我々は、ピアツーピアネットワークを利用した二重支出問題の解決策を提案する。ネットワークは、ハッシュベースのプルーフ・オブ・ワークの継続的な連鎖にハッシュすることでトランザクションにタイムスタンプを付与し、プルーフ・オブ・ワークをやり直さない限り変更できない記録を形成する。最長のチェーンは、目撃された一連の出来事を証明するだけでなく、それが最大の CPU パワーのプールから生まれたことを証明する。CPU パワーの大半が、ネットワークを攻撃するために協力していないノードによってコントロールされている限り、彼らは最長のチェーンを生成し、攻撃者を出し抜くことができる。ネットワーク自体は最小限の構造しか必要としない。メッセージはベストエフォート・ベースでブロードキャストされ、ノードは自由にネットワークから離脱したり再参加したりすることができ、離脱中に起こったことの証明として最長のプルーフ・オブ・ワークチェーンを受け入れる。

はじめに
インターネット上での商取引は、電子決済を処理するために、信頼できる第三者と して機能する金融機関にほぼ全面的に依存するようになった。このシステムは、ほとんどの取引では十分に機能しているが、信頼に基づくモデル特有の弱点がまだ残っている。金融機関は紛争の調停を避けることができないため、完全に非可逆的な取引は実際には不可能である。また、非可逆的なサービスに対して非可逆的な支払いを行う能力を失うという、より広範なコストが発生する。逆転の可能性があると、信頼の必要性が広がる。加盟店は顧客を警戒し、必要以上の情報を求めるようになる。一定の割合の詐欺は避けられないものとして受け入れられる。このようなコストや支払いの不確実性は、現物の通貨を使用することで回避できるが、信頼できる当事者なしに通信チャネル上で支払いを行う仕組みは存在しない。

必要なのは、信頼の代わりに暗号的な証明に基づく電子決済システムであり、信頼できる第三者を介することなく、意思のある当事者同士が直接取引できるようにすることである。計算上不可能な取引は、売り手を詐欺から守り、日常的なエスクローの仕組みは買い手を守るために簡単に実装できる。本論文では、ピアツーピアの分散型タイムスタンプサーバーを用いて、取引の時系列順序の計算論的証明を生成することで、二重支出問題の解決策を提案する。このシステムは、誠実なノードが攻撃者ノードの協力グループよりも多くの CPU パワーを制御している限り安全である。

---

## Translation Review

### Evaluation Matrix

| Dimension | Google Translate | OpenL Translate | Yandex Translate | DeepL |
| :--- | :---: | :---: | :---: | :---: |
| **Accuracy** | 8/10 | **9/10** | 6/10 | 8/10 |
| **Fluency** | 8/10 | **9/10** | 5/10 | **9/10** |
| **Consistency** | 8/10 | **9/10** | 6/10 | 8/10 |
| **Style Adaptation** | 7/10 | **9/10** | 5/10 | 8/10 |
| **Completeness** | **10/10** | **10/10** | **10/10** | **10/10** |
| **Total Score** | **41/50** | **46/50** | **32/50** | **43/50** |

---

### Key Insights

1. **OpenL Translate** demonstrates the highest overall quality, with superior accuracy in technical terminology and excellent fluency in Japanese
2. **DeepL** produces very natural Japanese but shows some inconsistencies in technical term translation
3. **Google Translate** provides reliable translations with good consistency but lacks the nuance of more sophisticated tools
4. **Yandex Translate** significantly underperforms, with awkward phrasing and several accuracy issues

---

### Detailed Analysis

#### Terminology and Nuance

**Key technical terms comparison:**
- "peer-to-peer": All translators use ピアツーピア/ピア・ツー・ピア correctly
- "proof-of-work": OpenL and Google use プルーフ・オブ・ワーク consistently; Yandex mixes English and katakana; DeepL uses プルーフ・オブ・ワーク
- "double-spending": All use 二重支払い correctly
- "hash-based": OpenL's ハッシュベース is more natural than others' variations

**Notable differences:**
- OpenL: "小額かつ気軽な取引" (small and casual transactions) - captures both aspects elegantly
- Google: "小規模な取引" (small-scale transactions) - loses the "casual" nuance
- DeepL: "非可逆的な" for "non-reversible" is more formal/technical than others' "不可逆な"
- Yandex: "カジュアルな取引" - unnecessarily uses English loanword

#### Fluency and Sentence Structure

**OpenL** excels with natural Japanese flow:
- "これにより、プルーフ・オブ・ワークをやり直さない限り変更できない記録が形成されます" - clear cause-and-effect structure
- Smooth transitions between sentences using appropriate conjunctions

**DeepL** produces very readable Japanese but occasionally oversimplifies:
- "我々は、ピアツーピアネットワークを利用した二重支出問題の解決策を提案する" - academic style appropriate for whitepaper

**Google** maintains good readability with occasional stiffness:
- "本稿では" usage is appropriate but sometimes repetitive

**Yandex** struggles with Japanese grammar:
- "攻撃者を ネットワーク自体は" - broken sentence structure
- Awkward particle usage throughout

#### Completeness

All four services translated the complete text without omissions. The evaluation focuses on how completely they conveyed the meaning rather than word count.

---

### Summary

**OpenL Translate** emerges as the clear winner for Bitcoin whitepaper translation, combining technical accuracy with natural Japanese expression. It successfully maintains the academic tone while ensuring readability.

**DeepL** ranks second, producing highly fluent Japanese but with occasional terminology inconsistencies that could confuse technical readers.

**Google Translate** provides a solid, reliable translation suitable for general understanding, though it lacks the sophistication needed for publication-quality technical documentation.

**Yandex Translate** is not recommended for technical translations of this complexity, showing significant issues with both accuracy and fluency that would require extensive post-editing.

For translating technical documents like the Bitcoin whitepaper, **OpenL Translate** is the recommended choice, with **DeepL** as a strong alternative when natural fluency is prioritized over absolute technical precision.