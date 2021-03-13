---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4b5d049ac32dba71c6ed04ec5cc4533eddb382b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790086"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Emails["{itemEmail-id}"]
    .Request()
    .DeleteAsync();

```