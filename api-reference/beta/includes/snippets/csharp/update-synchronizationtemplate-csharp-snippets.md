---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cca01768b7aeaf0a943d177828a85664a9331ef82ab22c96a5310a7c879251d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104477"
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