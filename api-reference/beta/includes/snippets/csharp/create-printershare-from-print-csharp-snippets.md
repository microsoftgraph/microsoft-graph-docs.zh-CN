---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b172fd43445bc87218b11fbc41beb3144ed875ce75dbcbb11bebdec57abdbf0b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903313"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShare = new PrinterShare
{
    Name = "name-value",
    AdditionalData = new Dictionary<string, object>()
    {
        {"printer@odata.bind", "https://graph.microsoft.com/beta/print/printers/{id}"}
    }
};

await graphClient.Print.Shares
    .Request()
    .AddAsync(printerShare);

```