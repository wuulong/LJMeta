# LJMeta
 Legal Judgment Metadata

# Spec
- [判決書 Meta Data 規格書](https://github.com/wuulong/LJMeta/blob/main/%E5%88%A4%E6%B1%BA%E6%9B%B8%20Meta%20Data%20%E8%A6%8F%E6%A0%BC%E6%9B%B8.md)

# 一般
- 構思：[AIQA-法律判決書](https://github.com/wuulong/LJMeta/blob/main/AIQA-%E6%B3%95%E5%BE%8B%E5%88%A4%E6%B1%BA%E6%9B%B8.md)

# 版本歷史
- V0.0.1(目前)：
	- 初始規格，搭配第一個判決書範例

# 範例
- 來源： [臺灣新竹地方法院 113 年家親聲字第 415 號民事判決](https://judgment.judicial.gov.tw/FJUD/data.aspx?ty=JD&id=SCDV,113%2c%e5%ae%b6%e8%a6%aa%e8%81%b2%2c415%2c20241111%2c1)

	- [臺灣新竹地方法院 113 年家親聲字第 415 號民事判決.md](https://github.com/wuulong/LJMeta/blob/main/judgment/%E8%87%BA%E7%81%A3%E6%96%B0%E7%AB%B9%E5%9C%B0%E6%96%B9%E6%B3%95%E9%99%A2%20113%20%E5%B9%B4%E5%AE%B6%E8%A6%AA%E8%81%B2%E5%AD%97%E7%AC%AC%20415%20%E8%99%9F%E6%B0%91%E4%BA%8B%E5%88%A4%E6%B1%BA.md)
	- [臺灣新竹地方法院 113 年家親聲字第 415 號民事判決_CM.json](https://github.com/wuulong/LJMeta/blob/main/judgment/%E8%87%BA%E7%81%A3%E6%96%B0%E7%AB%B9%E5%9C%B0%E6%96%B9%E6%B3%95%E9%99%A2%20113%20%E5%B9%B4%E5%AE%B6%E8%A6%AA%E8%81%B2%E5%AD%97%E7%AC%AC%20415%20%E8%99%9F%E6%B0%91%E4%BA%8B%E5%88%A4%E6%B1%BA_CM.json)
	- [臺灣新竹地方法院 113 年家親聲字第 415 號民事判決_M.json](https://github.com/wuulong/LJMeta/blob/main/judgment/%E8%87%BA%E7%81%A3%E6%96%B0%E7%AB%B9%E5%9C%B0%E6%96%B9%E6%B3%95%E9%99%A2%20113%20%E5%B9%B4%E5%AE%B6%E8%A6%AA%E8%81%B2%E5%AD%97%E7%AC%AC%20415%20%E8%99%9F%E6%B0%91%E4%BA%8B%E5%88%A4%E6%B1%BA_M.json)

# 解析練習
## 透過 colab 載入 json, 做初步觀察
- [判決書 Meta Data1.ipynb](https://drive.google.com/open?id=1VT77m8EsYYI9wGJU6YN6D8RBstZA6CJe&usp=drive_copy)
- [判決書 Meta Data2.ipynb](https://drive.google.com/open?id=1xyErJ0vuT3hXIBtPzoz_RkLxP7mN32C_&usp=drive_copy)


# 手動建構 metadata
- 先搜尋到想要的判決書，手動存成 md 檔
	- [司法院法學資料檢索系統](https://lawsearch.judicial.gov.tw/default.aspx)
		- 找到後點選，去格式引用
- 在 LLM 工具（如 Google AI Studio），匯入 規格書與要建構的判決書.md，要 LLM 生成
	- prompt 範例:請根據判決書 meta data 規格書，針對附件的判決書，產生 通用 Meta data 與 內容 meta data 
- 手動將 json 複製出來存檔



# 參考
- 判決書的 meta data 也可與 [law_meta](https://github.com/wuulong/law_meta) 接合
