---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 550391f3de7046eb890663a551dddb6278717145
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771286"
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