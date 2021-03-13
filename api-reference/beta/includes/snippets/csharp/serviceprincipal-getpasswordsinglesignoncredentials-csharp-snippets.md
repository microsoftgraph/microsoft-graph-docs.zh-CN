---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27d3943aad28b57c9367aa5322aa13847a42c0a0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793265"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var id = "5793aa3b-cca9-4794-679a240f8b58";

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .GetPasswordSingleSignOnCredentials(id)
    .Request()
    .PostAsync();

```