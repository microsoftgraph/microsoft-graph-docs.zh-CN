---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7c50deeb46aed033aa32bdba8efa3ad9511e5d8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771846"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTaskTrigger = new PrintTaskTrigger
{
    Event = PrintEvent.JobStarted,
    AdditionalData = new Dictionary<string, object>()
    {
        {"definition@odata.bind", "https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}"}
    }
};

await graphClient.Print.Printers["{printer-id}"].TaskTriggers
    .Request()
    .AddAsync(printTaskTrigger);

```