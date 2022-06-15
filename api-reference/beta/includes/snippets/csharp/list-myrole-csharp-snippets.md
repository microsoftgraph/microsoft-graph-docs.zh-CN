---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c046d23fc6c5d09d8d4abe424f17f6b111793f3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096360"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var myRoles = await graphClient.TenantRelationships.ManagedTenants.MyRoles
    .Request()
    .GetAsync();

```