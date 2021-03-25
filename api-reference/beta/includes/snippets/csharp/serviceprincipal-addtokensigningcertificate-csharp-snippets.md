---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ca463d9efba5b515444a996a4af5d8d40dc734e
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202510"
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