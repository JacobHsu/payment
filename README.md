# payment

第三方支付：綠界、歐付寶、藍新  
[藍新金流](https://www.newebpay.com/)  
[API 文件下載](https://www.newebpay.com/website/Page/content/download_api)

用戶的流程

- 建立訂單 - 送出訂單 - → 轉址到第三方支付，並付款 - ← 轉回電商網站

建立訂單及訂單號碼  
建立金流需要的表單  
透過表單轉址到金流網站 →
← 接收回傳

1. 前端的回傳 (藍新金流的名稱 Return URL) : 建議通過 https
2. 後端的回傳 (藍新金流的名稱 Notify URL) : 必要使用 443 port

## Usage

`$ npm start`  
http://localhost:3000/

## Note

[express](https://expressjs.com/zh-tw/starter/installing.html)  
`$ npm install express --save` 

[將模板引擎用於 Express](https://expressjs.com/zh-cn/guide/using-template-engines.html)  
[pug](https://www.npmjs.com/package/pug)  

日誌組件 [morgan](https://www.npmjs.com/package/morgan)  
> morgan是express默認的日誌中間件，也可以脫離express，作為node.js的日誌組件單獨使用。
`$ npm install morgan --save` 

[cookie-parser](https://www.npmjs.com/package/cookie-parser) 
> 是Express的中間件，用來實現cookie的解析  

[body-parser](https://www.npmjs.com/package/body-parser)
> express中間件，作用是對post請求的請求體進行解析

## References

https://github.com/Wcc723/spgateway_payment_demo