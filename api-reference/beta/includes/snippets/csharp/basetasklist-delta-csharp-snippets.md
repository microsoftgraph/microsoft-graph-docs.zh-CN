---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20a97e561cfac4e8e9e9a289a9e7c79231918532
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525252"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Tasks.Lists.Delta
    .Request()
    .GetAsync();

```