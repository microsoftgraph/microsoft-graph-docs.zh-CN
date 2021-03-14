---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bb710bb91e1dbdf06ed9dd2da14181f7200af69
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806381"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = await graphClient.Applications["{application-id}"]
    .Request()
    .GetAsync();

```