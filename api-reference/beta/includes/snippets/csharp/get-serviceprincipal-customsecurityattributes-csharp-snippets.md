---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3dd2f64086fa41011a88613f98216cdbf8ed2d48
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226259"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .Request()
    .Select("customSecurityAttributes")
    .GetAsync();

```