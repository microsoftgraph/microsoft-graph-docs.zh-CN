---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a825a4ede0c0ffcd4c70d08a48067bfc5c5248f0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807435"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Planner.Rosters["{plannerRoster-id}"].Members
    .Request()
    .GetAsync();

```