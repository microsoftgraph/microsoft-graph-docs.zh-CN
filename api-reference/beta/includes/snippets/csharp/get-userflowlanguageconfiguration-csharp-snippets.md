---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e8adc4ce6e6d0dafa73acb09b2b82b71a75c69a
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274700"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languages = await graphClient.Identity.B2xUserFlows["B2X_1_PartnerSignUp"].Languages
    .Request()
    .GetAsync();

```