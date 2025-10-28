# Hello, I'm Datarchpy 👋

Welcome to my GitHub portfolio! Here you can find my projects showcasing my skills and experience in software development, data analysis, and machine learning. / 私のGitHubポートフォリオへようこそ！ここでは、ソフトウェア開発、データ分析、機械学習に関するスキルと経験を紹介するプロジェクトを掲載しています。

---

## 🛠️ Skills / 技術スキル
[![My Skills](https://skillicons.dev/icons?i=py&theme=dark)](https://skillicons.dev)
- **Programming Languages / プログラミング言語**: Python, TypeScript, JavaScript, C++
  - **Frameworks / フレームワーク**:
    - **Web**: Next.js, React, FastAPI
    - **ML/AI**: TensorFlow, PyTorch, Streamlit
  - **Tools / ツール**: Git, Firebase, Docker
  - **BI Tools / BIツール**: Tableau, PowerBI, Looker studio

---

## 🌐 Web Applications / Webアプリケーション

  ### **Action Activation Therapy - 行動活性化療法支援アプリ**
  [![Skills Used](https://skillicons.dev/icons?i=nextjs,typescript,python,fastapi,firebase&theme=dark)](https://skillicons.dev)

  機械学習を活用した行動最適化支援Webアプリケーション。行動と気分の記録・可視化、ML による気分低下の予兆検知機能を提供。

  - **課題**: 行動活性化療法における行動記録と気分予測を支援するフルスタックアプリケーションの構築。
  - **使用技術**:
    - **Frontend**: Next.js 14 (App Router), TypeScript, Tailwind CSS, Recharts
    - **Backend**: FastAPI, SQLite, SQLAlchemy
    - **Auth**: Firebase Authentication
    - **ML**: scikit-learn (気分予測モデル)
    - **Infrastructure**: CI/CD (GitHub Actions), Vercel, Railway
  - **主な機能**:
    - Firebase による認証・認可
    - 行動と気分のデータ可視化
    - 機械学習による気分低下の予兆検知（開発中）
    - PWA対応（スマホアプリのような体験）
  - **品質管理**: テストカバレッジ62%、27テストケース実装、CI/CD自動化
  - [📦 Repository](https://github.com/Datarchpy/action-activation-therapy)
  - [🚀 Live Demo](https://datarchpy-action-activation-therapy.vercel.app/)

  ---
  
## 🤖 Machine Learning Projects / 機械学習プロジェクト

  ### **arXiv Query Expander Fine-tuning - GPT-3.5ファインチューニングによるarXiv検索最適化** ⭐
  [![Skills Used](https://skillicons.dev/icons?i=python&theme=dark)](https://skillicons.dev)

  GPT-3.5のファインチューニングにより、arXiv論文検索のクエリ拡張精度を大幅に向上させたプロジェクト。データセット拡大と過学習対策により    
、低コストで高い性能改善を実現。

  - **課題**: 小規模データセット（80サンプル）でのファインチューニングが過学習を引き起こし、性能が悪化（88.9% →
  61.1%）。この問題を解決し、検索精度を向上させる。
    - **成果**:
      - **検索成功率**: 81.8% → **92.7%** (+10.9% 改善) ✨
      - **検索品質（Rerank Score）**: 0.7776 → **0.8815** (+13.4% 改善) ✨
      - **データセット拡大**: 80 → **252サンプル** (3.15倍)
      - **総コスト**: わずか **$4.13** で大幅な性能向上を達成
    - **使用技術**:
      - **Fine-tuning**: OpenAI GPT-3.5 Fine-tuning API
      - **Data Pipeline**: Python, arxiv API, Cohere Rerank API
      - **Tools**: Git, OpenAI SDK
    - **技術的ハイライト**:
      - **過学習対策の実装**: epochs削減（3→1）、learning rate調整（0.1）により過学習を軽減
      - **データ品質改善**: 引用符削除により成功率90.25%を達成（v1/v2: 45-55% → v3: 90.25%）
      - **自動化パイプライン**: バッチ処理によるデータ収集、品質フィルタリング、評価の完全自動化
      - **API制限対応**: Cohere Trial keyのrate limit（10 calls/分）を回避する遅延機構を実装
      - **包括的なドキュメント**: 実験レポート、ポートフォリオサマリー、GitHub公開手順を完備
    - **問題解決プロセス**:
      1. 過学習の診断（training loss = 0.00）
      2. データセット拡大（80 → 252サンプル）
      3. データクリーンアップ（引用符28.8% → 0%）
      4. ハイパーパラメータ最適化
      5. 性能評価とベースライン比較
    - [📦 Repository](https://github.com/Datarchpy/arxiv-query-expander-finetuning)
    - [📊 Portfolio Summary](https://github.com/Datarchpy/arxiv-query-expander-finetuning/blob/main/portfolio/PORTFOLIO_SUMMARY.md)
    - [📝 Experiment 
  Report](https://github.com/Datarchpy/arxiv-query-expander-finetuning/blob/main/portfolio/EXPERIMENT_REPORT_FINAL.md)

  ---
  


## 🏛️ Competitions & Achievements / コンペティションと成果

### 【Kaggle】

- **Stanford RNA 3D Folding（コンペティション）**
    - **🥈銀メダル獲得**
    - **課題**: RNAの3D構造予測コンペティション。
    - **使用技術**: RhoFold, DRFold, Boltz。

#### **RhoFold+ Inference Optimization - RNA 3D構造予測の推論最適化** ⭐
  [![Skills Used](https://skillicons.dev/icons?i=python,pytorch&theme=dark)](https://skillicons.dev)

  RhoFold+（RNA
  3D構造予測モデル）の推論速度を**29.3%向上**させた最適化プロジェクト。段階的な最適化手法の実装と評価を通じて、実用的な高速化を達成。       

  - **課題**: RhoFold+の推論時間が長く、Kaggle環境のGPU時間制限内での実行が困難。Recyclingメカニズムの計算コストが高い。
  - **使用技術**:
    - **Deep Learning**: PyTorch 2.0+, CUDA 11.8
    - **最適化手法**: Smart Recycling（早期停止）、RNA-FMキャッシング、Mixed Precision
    - **プロファイリング**: PyTorch Profiler、メモリ解析
    - **環境**: Kaggle Notebooks (Tesla P100/T4 GPU)
  - **成果**:
    - 推論時間: 6.912秒 → 5.347秒（**29.3%改善**）
    - GPUメモリ: 814.7MB → 780.5MB（4.2%削減）
    - 実行サイクル数: 10サイクル → 平均4サイクル（**60%削減**）
    - 精度維持: TM-score 0.3937 → 0.3952（精度を保ちながら高速化）
    - 長い配列（100nt）では**最大401.6%の高速化**
  - **技術的ハイライト**:
    - 3フェーズの段階的最適化アプローチ
    - 構造収束監視による動的早期停止（RMSD < 0.5Å）
    - 失敗した最適化の詳細分析（Mixed PrecisionがP100/T4で逆効果になった理由など）
    - 包括的なドキュメント作成（技術解説、実験結果分析）
  - [📦 Repository](https://github.com/Datarchpy/rhofold-optimization)
  - [📊 Kaggle Results](https://github.com/Datarchpy/rhofold-optimization/tree/master/kaggle_optimization/results)

  ---


- **LLM Prompt Recovery**
  - **課題**: 大規模言語モデル（LLM）からのプロンプト復元。モデル間のパフォーマンス差を比較検証。
  - **使用技術**: Transformer, Hugging Face。

- **The Learning Agency Lab - PII Data Detection**
  - **課題**: 個人情報検出モデルの構築。正確性向上のためデータ拡張を実施。
  - **使用技術**: BERT, SpaCy。

- **RSNA 2024 Lumbar Spine Degenerative Classification**
  - **課題**: 医療画像を用いた腰椎退行性変性の分類。
  - **使用技術**: ResNet50, TensorFlow, CLAHE。

- **AI Mathematical Olympiad - Progress Prize 1**
  - **課題**: 数学問題の解法生成モデルの開発と評価。
  - **使用技術**: GPT-3, 自然言語処理。

- **LMSYS - Chatbot Arena Human Preference Predictions**
  - **課題**: チャットボット間でのユーザー選好予測モデルの構築。
  - **使用技術**: RLHF, Scikit-learn。

- **Eedi - Mining Misconceptions in Mathematics**
  - **課題**: 数学教育データにおける誤解ポイントの分析。
  - **使用技術**: XGBoost, Python。

---
### 【atmaCup】
- **#19 atmaCup 「Top14%」**
  - **課題**: 実店舗とECサイトのセッションデータによる購買予測。
  - **使用技術**: LightGBM, LSTM。
  - [実装コード](https://github.com/Datarchpy/atmaCup19)

- **#18 Turing × atmaCup 「Top12%」**
  - **課題**: NLPを用いたテキストデータの感情分析と分類モデルの構築。
  - **使用技術**: ConvNext, LightGBM。
  - [実装コード](https://github.com/Datarchpy/Turing_atmaCup18)
  

- **#17 [初心者歓迎] atmaCup 「Top21%」**
  - **課題**: 自然言語処理を用いた衣服レビュー推薦予測。
  - **使用技術**: Devarta, LightGBM。
  - [実装コード](https://github.com/Datarchpy/atmaCup17)

- **atmaCup #16 in collaboration with RECRUIT 「Top14%」**
  - **課題**: レコメンデーションシステムの構築。特徴量エンジニアリングに注力。
  - **使用技術**: XGBoost, PCA。
---
### 【MDXQ2023】
- **PBL02 不良個所自動検出（製造）「AI課題優秀賞」**
  - **課題**: 製造ラインで発生する不良個所を自動検出するアルゴリズムを開発。精度向上のため、アノテーションデータの品質向上とデータ拡張を実施。
  - **使用技術**: TensorFlow, OpenCV, モデル精度検証に交差検証を適用。

- **PBL06 新規事業提案/組織変革（食品製造小売企業）「総合第4位」**
  - **課題**: 食品製造業の新規事業立案に携わり、データに基づく市場分析を実施。
  - **使用技術**: Tableau, Pythonで市場データを視覚化し、売上予測を実施。

- **PBL03 収益改善（店舗運営型）「DS課題優秀賞」**
  - **課題**: 店舗運営における利益改善のため、売上データと来店データを分析。
  - **使用技術**: SQL, Python, Tableauで在庫最適化と利益分析を実施。

- **PBL05 工数予測（製造）「AI課題優秀賞」**
  - **課題**: 製造ラインの工数を正確に予測するアルゴリズムを設計。
  - **使用技術**: Python, LightGBM, AutoML(AutoGluon)
  - [実装コード](https://github.com/Datarchpy/pbl05_mdxq2024)
---
### 【AtCoder Heuristic Contest】
- **AtCoder Heuristic Contest 048**
  - **課題**: xxxxx。
  - **使用技術**: xxxx。
  - [実装コード](https://github.com/Datarchpy/Stanford-RNA-3D-Folding)
---

## 🏆 Certifications & Awards / 認定資格と賞給
- **JDLA Deep Learning for ENNGINEER 2024#2** 
---

## 📣 Contact / 連絡先
Feel free to reach out to me via [LinkedIn](https://www.linkedin.com/in/your-profile) or [Email](mailto:your-email@example.com). / [LinkedIn](https://www.linkedin.com/in/your-profile)または[Email](mailto:your-email@example.com)でお気軽にご連絡ください。

[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=datarchpy&show_icons=true&theme=onedark)](https://github.com/anuraghazra/github-readme-stats)




