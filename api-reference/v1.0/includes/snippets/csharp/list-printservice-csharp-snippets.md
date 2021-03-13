---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ddaa51f960fd65909793ac85e1b609212ff2830
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777227"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var services = await graphClient.Print.Services
    .Request()
    .GetAsync();

```