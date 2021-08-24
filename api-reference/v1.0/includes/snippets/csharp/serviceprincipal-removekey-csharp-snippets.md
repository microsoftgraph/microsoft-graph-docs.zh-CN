---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bea2c429c94393e5cc4f58a8cbcaad021539d67dddfb0791fcec10a46108b947
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219996"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyId = Guid.Parse("f0b0b335-1d71-4883-8f98-567911bfdca6");

var proof = "eyJ0eXAiOiJ...";

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .RemoveKey(keyId,proof)
    .Request()
    .PostAsync();

```