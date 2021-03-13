---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a37356ea908dc155f35d57c5e73c4bd1d65dd774
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808544"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationTemplate = new SynchronizationTemplate
{
    Id = "Slack",
    ApplicationId = Guid.Parse("{id}"),
    FactoryTag = "CustomSCIM"
};

await graphClient.Applications["{application-id}"].Synchronization.Templates["{synchronizationTemplate-id}"]
    .Request()
    .Header("Authorization","Bearer <token>")
    .PutAsync(synchronizationTemplate);

```