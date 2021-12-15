---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b3a86b97dc90d77b7cfaf89e8097f2ff66e1a55
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524542"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Tasks.Lists.AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAu.Tasks.AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT
    .Request()
    .DeleteAsync();

```