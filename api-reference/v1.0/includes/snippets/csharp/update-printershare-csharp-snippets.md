---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc990deb4f02a7326f9540fe2ae5100a892bf9e12531beeb82a5b45d65f87cb6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902237"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShare = new PrinterShare
{
    DisplayName = "PrinterShare Name",
    AllowAllUsers = false,
    AdditionalData = new Dictionary<string, object>()
    {
        {"printer@odata.bind", "https://graph.microsoft.com/v1.0/print/printers/{printerId}"}
    }
};

await graphClient.Print.Shares["{printerShare-id}"]
    .Request()
    .UpdateAsync(printerShare);

```