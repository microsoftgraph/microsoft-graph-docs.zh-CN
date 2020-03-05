---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf49a45e64765614cdfb34209f065ea96a4bafb8
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41558818"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicies = await graphClient.ServicePrincipals["{id}"].ClaimsMappingPolicies
    .Request()
    .GetAsync();

```