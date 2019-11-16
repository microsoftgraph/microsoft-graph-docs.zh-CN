---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec219b73741e988b9e0e42f4b90e911eeca6369a
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37637807"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Planner.Tasks
    .Request()
    .GetAsync();

```