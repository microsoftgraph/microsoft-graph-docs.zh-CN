---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41bdfaebcc091a4d7e4c2f27b37f62207a39b7d8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781267"
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