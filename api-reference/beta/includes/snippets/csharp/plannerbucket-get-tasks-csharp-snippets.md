---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81e8ecbde8cbf16abb16951c4f1e2b3816441779
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783628"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Buckets["{plannerBucket-id}"].Tasks
    .Request()
    .GetAsync();

```