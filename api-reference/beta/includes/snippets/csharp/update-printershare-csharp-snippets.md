---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c53fa2e214ee0cba43f172a38d05813c8e5db9f7
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947631"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShare = new PrinterShare
{
    Name = "ShareName",
    AdditionalData = new Dictionary<string, object>()
    {
        {"printer@odata.bind","https://graph.microsoft.com/beta/print/printers/{id}"}
    }
};

await graphClient.Print.PrinterShares["{id}"]
    .Request()
    .UpdateAsync(printerShare);

```