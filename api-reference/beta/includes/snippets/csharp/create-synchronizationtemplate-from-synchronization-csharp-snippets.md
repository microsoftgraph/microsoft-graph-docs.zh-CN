---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bbce311abd837f04462dff26da907a2b2cdc043b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463575"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationTemplate = new SynchronizationTemplate
{
    Id = "SCIM-Test1",
    ApplicationId = "{id}",
    FactoryTag = "CustomSCIM"
};

await graphClient.Applications["{id}"].Synchronization.Templates
    .Request()
    .AddAsync(synchronizationTemplate);

```