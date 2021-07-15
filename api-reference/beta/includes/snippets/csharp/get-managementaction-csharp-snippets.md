---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5245673a738826d9fc8ff6fb5b4b6b3bc438e3f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442130"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementAction = await graphClient.TenantRelationships.ManagedTenants.ManagementActions["{managedTenants.managementAction-id}"]
    .Request()
    .GetAsync();

```