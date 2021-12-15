---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e13771366ee77df6d4081b2d5a64f9ba3132fca
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var lists = await graphClient.Me.Tasks.Lists
    .Request()
    .GetAsync();

```