---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24e716e41a462aca1771204a951e62b38be891ed7587aa455ce0a16fb063dfc1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219180"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TenantRelationships.ManagedTenants.TenantTags["{managedTenants.tenantTag-id}"]
    .Request()
    .DeleteAsync();

```