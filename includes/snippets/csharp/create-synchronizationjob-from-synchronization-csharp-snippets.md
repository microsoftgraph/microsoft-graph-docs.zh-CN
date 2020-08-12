---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa1edc171492f070bf57df82bbb4f5d50c1eb51e
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643789"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationJob = new SynchronizationJob
{
    TemplateId = "aws"
};

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs
    .Request()
    .AddAsync(synchronizationJob);

```