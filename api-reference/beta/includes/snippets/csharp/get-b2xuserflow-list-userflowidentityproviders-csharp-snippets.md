---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fefab69b5ce645b26f89d46751f8194558757ee82350c56959aa42241c7b3c53
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162144"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowIdentityProviders = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].UserFlowIdentityProviders
    .Request()
    .GetAsync();

```