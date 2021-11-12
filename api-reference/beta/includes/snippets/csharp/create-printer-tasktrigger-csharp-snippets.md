---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 391279b9e4f177d367e66dda48a583ee7111a76abe4554fede38a3bd81c4d361
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161855"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTaskTrigger = new PrintTaskTrigger
{
    Event = PrintEvent.JobStarted,
    AdditionalData = new Dictionary<string, object>()
    {
        {"definition@odata.bind", "https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c"}
    }
};

await graphClient.Print.Printers["{printer-id}"].TaskTriggers
    .Request()
    .AddAsync(printTaskTrigger);

```