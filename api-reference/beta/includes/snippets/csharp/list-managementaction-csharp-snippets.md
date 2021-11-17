---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 143d37585e051a35ab5f70264fc9a6f7720ef1ff8dd9a1a702d7841fb57a8e83
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163400"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementActions = await graphClient.TenantRelationships.ManagedTenants.ManagementActions
    .Request()
    .GetAsync();

```