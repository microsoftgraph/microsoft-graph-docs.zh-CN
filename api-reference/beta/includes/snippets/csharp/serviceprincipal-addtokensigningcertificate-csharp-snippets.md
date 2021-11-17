---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f491c6109ed71cc4249758261e65e5639e4b82b47a3395700d5d25d2dfc8273
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "CN=customDisplayName";

var endDateTime = DateTimeOffset.Parse("2024-01-25T00:00:00Z");

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .AddTokenSigningCertificate(displayName,endDateTime)
    .Request()
    .PostAsync();

```