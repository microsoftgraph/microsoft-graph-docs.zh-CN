---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae7e704a8608c1a5b8a67745e36050d6e1aadb2c
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44216726"
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

await graphClient.Print.Shares["{id}"]
    .Request()
    .UpdateAsync(printerShare);

```