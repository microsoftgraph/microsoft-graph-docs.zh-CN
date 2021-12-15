---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cbaee800c9cc70766311828e16dfc6630e740f2
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525453"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Tasks.Lists.AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNm.Tasks
    .Request()
    .GetAsync();

```