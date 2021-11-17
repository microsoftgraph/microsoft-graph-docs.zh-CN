---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69030e55f12f9d919d3c310cfa31087023d7804ea5fdfaf7f0d5fd070bb6df62
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219971"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"].Schema.Directories["{directoryDefinition-id}"]
    .Discover()
    .Request()
    .PostAsync();

```