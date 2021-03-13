---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd9dfddc88c575ec6a410c221dab81feb4ccad37
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797644"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerProgressTaskBoardTaskFormat = await graphClient.Planner.Tasks["{plannerTask-id}"].ProgressTaskBoardFormat
    .Request()
    .GetAsync();

```