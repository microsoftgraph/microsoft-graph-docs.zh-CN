---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 31db2893c05aab868ca58ccf0d3906f87d06c44e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456569"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversation = await graphClient.Groups["02bd9fd6-8f93-4758-87c3-1fb73740a315"].Conversations["AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="]
    .Request()
    .GetAsync();

```