---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c16ab265b8d1407644c1bb9b5001f120cd561c4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809115"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Schedule.SchedulingGroups["{schedulingGroup-id}"]
    .Request()
    .DeleteAsync();

```