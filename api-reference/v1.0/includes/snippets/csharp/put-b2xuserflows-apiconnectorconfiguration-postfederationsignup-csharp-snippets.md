---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b81672cd4c0dbcbc13a405b8f75bda17b0fac047e30b40bc87769ca3f69d553
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105423"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].PostFederationSignup.Reference
    .Request()
    .PutAsync("{id}");

```