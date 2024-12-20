# PaymentTerminalManagerAPI

API service to support PaymentTerminalManager methods

# بانک ها

- سداد بانک ملی برای دستگاه های بلو برد (Bank Meli)
- به پرداخت بانک ملت (Behpardakht, Bank Melat)
- سامان کیش (SamanKish)
- اقتصاد نوین

# نحوه فراخوانی

نمونه کد ارسال مبلغ ۱۰۰۰۰ ریال به ترمینال به پرداخت با آی پی 1.1 و دریافت نتیجه

```cs
PaymentTerminalManager.TransactionOperation to = new PaymentTerminalManager.TransactionOperation();
var result = to.SendToTerminal(SupportedTerminal.BEHPARDAKHT, new PaymentTerminalManager.dto.SendToTerminal {
    IP = "192.168.1.1",
    Port = 1024,
    Price = 10000,
    RequestId = "1"
});
```

---

# Swagger document links

assume server ip address is 192.168.1.1

http://192.160.1.1/swagger/index.html

<a href="https://www.coffeebede.com/amirfahmideh"><img class="img-fluid" src="https://coffeebede.ir/DashboardTemplateV2/app-assets/images/banner/default-yellow.svg" /></a>
