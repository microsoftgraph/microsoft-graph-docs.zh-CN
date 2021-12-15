---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cb8765d7defb3067192800e615d145e97a39d06
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525417"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var aQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAADG6BbDxY = await graphClient.Me.Tasks.Lists.AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAADG6BbDxY
    .Request()
    .GetAsync();

```