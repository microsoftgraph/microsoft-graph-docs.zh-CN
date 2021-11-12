---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ca15f66da78de22696b9f8676bcb2d384711160f5dc4279d5e4da61fa31a0b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333914"
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