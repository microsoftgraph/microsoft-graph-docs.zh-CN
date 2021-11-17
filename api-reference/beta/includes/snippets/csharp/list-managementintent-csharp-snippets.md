---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf169c50bef50231b2bc2de44b3ecb2c3f83951481d245320f093b4f76499332
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161214"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementIntents = await graphClient.TenantRelationships.ManagedTenants.ManagementIntents
    .Request()
    .GetAsync();

```