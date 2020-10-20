---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b27a9f0711759f53e42f7501a4f95c32128fb4eb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608674"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Events["{id}"]
    .DismissReminder()
    .Request()
    .PostAsync();

```