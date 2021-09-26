---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ba93870408a4ce161c9c6787f65a6ac085c800f0677e73d864fa4620a1488c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161438"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cIdentityUserFlow = new B2cIdentityUserFlow
{
    Id = "Customer",
    UserFlowType = UserFlowType.SignUpOrSignIn,
    UserFlowTypeVersion = 3f
};

await graphClient.Identity.B2cUserFlows
    .Request()
    .AddAsync(b2cIdentityUserFlow);

```