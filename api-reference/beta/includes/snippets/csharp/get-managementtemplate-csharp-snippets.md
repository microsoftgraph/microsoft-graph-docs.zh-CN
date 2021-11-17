---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1a30d9ca7f8375792ae776eef63d291007be6436e92d7ca2ad17b757b426a56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277605"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementTemplate = await graphClient.TenantRelationships.ManagedTenants.ManagementTemplates["{managedTenants.managementTemplate-id}"]
    .Request()
    .GetAsync();

```