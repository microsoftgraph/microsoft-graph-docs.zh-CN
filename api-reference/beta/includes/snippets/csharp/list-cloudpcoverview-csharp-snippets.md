---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7672c6100ff716c35d516f7fbd122526c46d2ff0
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441469"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcsOverview = await graphClient.TenantRelationships.ManagedTenants.CloudPcsOverview
    .Request()
    .GetAsync();

```