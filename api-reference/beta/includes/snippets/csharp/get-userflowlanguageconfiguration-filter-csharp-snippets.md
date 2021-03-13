---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 356db481e188adeb0ef5f6b39cdcee11cb4b8469
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798220"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languages = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages
    .Request()
    .Filter("isEnabled eq true")
    .GetAsync();

```