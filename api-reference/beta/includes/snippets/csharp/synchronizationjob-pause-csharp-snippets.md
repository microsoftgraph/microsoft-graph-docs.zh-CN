---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29fdda82cf964a647b43a9727746f328f2343c08bd4d8bdc71b20a733afc7742
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220581"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"]
    .Pause()
    .Request()
    .PostAsync();

```