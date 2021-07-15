---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebe47ea09222e7f355e1824c0940ea7ed520a9e0
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443021"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementIntents = await graphClient.TenantRelationships.ManagedTenants.ManagementIntents
    .Request()
    .GetAsync();

```