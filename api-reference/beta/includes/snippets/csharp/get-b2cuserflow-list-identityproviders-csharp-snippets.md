---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35a08cf15b0355ff77818d7f2c46ccf3e6e826a18e5d00c75509398989e95cd7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902857"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].IdentityProviders
    .Request()
    .GetAsync();

```