---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c681ebf491a6fe1c3d6fa9f74eb6623256bf060
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948230"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShare = new PrinterShare
{
    Name = "name-value",
    AdditionalData = new Dictionary<string, object>()
    {
        {"printer@odata.bind","https://graph.microsoft.com/beta/print/printers/{id}"}
    }
};

await graphClient.Print.PrinterShares
    .Request()
    .AddAsync(printerShare);

```