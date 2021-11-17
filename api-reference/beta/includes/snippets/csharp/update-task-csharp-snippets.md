---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c383610c2ca73e6708ed24d54386644214175032a592278ce6156e4d4b9f34bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333411"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTask = new PrintTask
{
    Status = new PrintTaskStatus
    {
        State = PrintTaskProcessingState.Completed,
        Description = "completed"
    }
};

await graphClient.Print.TaskDefinitions["{printTaskDefinition-id}"].Tasks["{printTask-id}"]
    .Request()
    .UpdateAsync(printTask);

```