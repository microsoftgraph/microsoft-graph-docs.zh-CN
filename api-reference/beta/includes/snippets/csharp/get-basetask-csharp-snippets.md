---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b8e89598cc9d7bd4e99ef5d68b1e4a7c3702fa4
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524796"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var aAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT--0qFRAqk3TNe0QAAAy35RwAA = await graphClient.Me.Tasks.Lists.AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt-6oC2JgAQCQ47jE5P--SoVECqTdM17RAAAB4mDIAAA=.Tasks.AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT--0qFRAqk3TNe0QAAAy35RwAA
    .Request()
    .GetAsync();

```