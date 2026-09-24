# AutoPPT 下載與版本紀錄

AutoPPT 是 Windows AI 簡報工作室，協助整理主題、大綱、素材、視覺風格並製作可編輯的 PowerPoint。

## 下載

前往 [最新版本](https://github.com/SamChengYo/AutoPPT-Releases/releases/latest)，目前版本 **0.6.1**，下載 `AutoPPT-Setup-0.6.1.exe`。本版修正大綱 JSON 錯誤，加入自動格式修正、實際生成進度與 SVG 自由構圖製作；詳見[版本說明](versions/v0.6.1.md)。

需要 Windows x64 與 Microsoft PowerPoint。原生 SmartArt 功能另需 Microsoft Excel 元件。安裝程式包含執行所需的 .NET、模型代理服務與 SVG 轉換器，不需另裝 Python；AI 功能需填入自己的供應商 API Key。

## 更新

本版在啟動頁自動檢查與下載更新，下載完成後由使用者選擇「重新啟動並安裝」，顯示安裝進度並於完成後自動開啟。網路失敗可先進入工作室。0.5.0 首次升級仍由舊版自動安裝流程控制；0.3.0 與更舊版可能顯示舊安裝精靈；0.1.0 使用者需手動安裝。0.6.0 為未發布的本機候選版本，公開更新由 0.5.0 直接升至 0.6.1。

更新保留本機專案及設定。若舊設定無法解密，程式會保留加密備份並提示重新輸入 API Key。解除安裝入口位於應用程式設定，預設保留本機資料。

版本的 `.sha256` 可用於檢查安裝檔完整性；`latest.yml` 與 `.blockmap` 供應用程式更新使用。安裝程式目前未簽章。

## 本倉庫內容

本倉庫僅提供安裝檔、更新資訊與版本說明。應用程式原始碼由獨立的私人倉庫管理。

若之後搬移下載主機，可在 AutoPPT 設定自訂 HTTPS 更新目錄。更新目錄須包含對應安裝檔、blockmap 及最後發布的 `latest.yml`。
