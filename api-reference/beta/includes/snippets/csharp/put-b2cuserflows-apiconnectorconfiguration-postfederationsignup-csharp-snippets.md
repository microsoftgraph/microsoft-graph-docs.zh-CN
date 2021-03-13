---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5052004bfcfc77049958c07c8e07fc873bb3cd1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805083"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].PostFederationSignup.Reference
    .Request()
    .PutAsync("{id}");

```