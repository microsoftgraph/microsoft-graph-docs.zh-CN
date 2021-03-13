---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85b6a890addb13cb367c05b4e718a8b2d30f0e3c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791210"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"].Schema.Directories["{directoryDefinition-id}"]
    .Discover()
    .Request()
    .PostAsync();

```