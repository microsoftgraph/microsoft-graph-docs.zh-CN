---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4783ca9f0735bcba76a3c9f90d30feb1bba12a347e0e1589ba810f61e221e0d9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279324"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyId = Guid.Parse("f0b0b335-1d71-4883-8f98-567911bfdca6");

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .RemovePassword(keyId)
    .Request()
    .PostAsync();

```