---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ee5db9a5fb2b1117ac7e9108dd6d2083ffd4b7f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952978"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var jobs = await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs
    .Request()
    .GetAsync();

```