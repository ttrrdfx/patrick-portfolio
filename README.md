# Patrick Profile

Patrick 的個人網站，使用純 HTML 與 CSS 製作。

## 專案內容

- `index.html`：網站內容與頁面結構
- `styles.css`：配色、排版與響應式樣式

這個專案目前沒有後端、資料庫或 Node.js server。

## 如何執行

### 方法一：使用 Python 本地伺服器（建議）

macOS 通常已經可以使用 Python。開啟終端機後執行：

```bash
cd /Users/patrick25/Documents/project/web-profile/profile
python3 -m http.server 4173
```

接著在瀏覽器開啟：

```text
http://localhost:4173
```

要停止伺服器，回到終端機按：

```text
Control + C
```

如果 `4173` 已被其他程式使用，可以換成其他連接埠，例如：

```bash
python3 -m http.server 8080
```

然後開啟 `http://localhost:8080`。

### 方法二：直接開啟 HTML

也可以直接雙擊 `index.html`，或在瀏覽器開啟：

```text
file:///Users/patrick25/Documents/project/web-profile/profile/index.html
```

目前網站是純靜態內容，因此這種方式也能顯示。不過使用 localhost 會更接近網站正式部署後的環境。

## 為什麼沒有 server.mjs 也能使用 localhost？

`localhost` 只代表「這台電腦」，不限定一定要使用 `server.mjs`。

這個專案可以透過 Python 內建的 `http.server` 暫時提供 HTML 與 CSS。指令執行期間，Python 就是本地靜態伺服器；停止指令後，localhost 網站也會停止。

## 修改後如何查看

儲存 `index.html` 或 `styles.css` 後，重新整理瀏覽器即可看到最新內容。若畫面沒有更新，可以使用強制重新整理：

```text
Command + Shift + R
```

## 正式發布

因為網站是純靜態網站，未來可以部署到 GitHub Pages、Cloudflare Pages、Netlify 或 Vercel，不需要額外後端。
