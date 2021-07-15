---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 409dff697077ccf66542e05c6c061515c25ff181
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441570"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcConnections = await graphClient.TenantRelationships.ManagedTenants.CloudPcConnections
    .Request()
    .GetAsync();

```