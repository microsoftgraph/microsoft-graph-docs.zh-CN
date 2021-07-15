---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0a45d6d2f87feb90116b26179b7cb7ae0325da1
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443049"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementTemplates = await graphClient.TenantRelationships.ManagedTenants.ManagementTemplates
    .Request()
    .GetAsync();

```