---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1a9e4a249679338f3be670b960e01f669a46e82
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440073"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcOverview = await graphClient.TenantRelationships.ManagedTenants.CloudPcsOverview["{managedTenants.cloudPcOverview-id}"]
    .Request()
    .GetAsync();

```