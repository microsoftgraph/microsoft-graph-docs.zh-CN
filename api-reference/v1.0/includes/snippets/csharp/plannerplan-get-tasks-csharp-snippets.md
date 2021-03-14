---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 915941fa2e05f440db4581a354cc4a4a7af68080
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778776"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Plans["{plannerPlan-id}"].Tasks
    .Request()
    .GetAsync();

```