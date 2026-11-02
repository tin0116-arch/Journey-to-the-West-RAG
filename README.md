# 🐒 悟空成長檔案館｜《西遊記》前七回 RAG 問答

## 專案內容
- `RAG01_西遊記_建立資料庫.ipynb`：讀取摘要、embedding、FAISS，輸出 `rag-data.zip`。
- `RAG02_西遊記_Gradio問答.ipynb`：從 GitHub raw 下載 `rag-data.zip`，用 AIsuite/Groq 及 Gradio 展示。
- `西遊記_第一至七回_章節摘要.zip`：依《西遊記》第一至第七回自行整理的章節摘要（不是原著全文）。
- `rag-data.zip`：**請先實際執行 RAG01，再將生成的 ZIP 上傳至 GitHub 根目錄**；本專案交付時不含已生成的索引。

## 操作方式
1. 把上述檔案上傳到 GitHub 公開 repository。
2. 用 Google Colab 開啟 RAG01，依序執行，手動選擇章節摘要 ZIP，下載產生的 `rag-data.zip`。
3. 上傳 `rag-data.zip` 至 GitHub repository 根目錄，確認檔案能被公開下載。
4. 在 RAG02 將 `RAG_ZIP_URL` 設成 `https://raw.githubusercontent.com/帳號/Repo/main/rag-data.zip`。
5. 在 Colab Secrets 設定 `Groq` 金鑰並啟用權限，依序執行 RAG02 至 Gradio。
6. 提交 RAG02 的 Colab 連結、介面與問答截圖、資料說明、人設背景。

## 使用資料與限制
來源：維基文庫《西遊記》https://zh.wikisource.org/wiki/西遊記 。章節摘要是作業整理內容，僅涵蓋第一至第七回，非原著逐字引用。RAG 的相似度不是答案的正確率。

## GitHub 中開啟 Colab
點 GitHub 的 `.ipynb` 檔可以預覽 Notebook。Colab 可透過 `https://colab.research.google.com/github/帳號/Repo/blob/main/RAG02_西遊記_Gradio問答.ipynb` 開啟；也可以直接在 Colab 以「檔案 → 在 GitHub 中開啟」選取。
