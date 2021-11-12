---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00558df4430745e42b54a527dc7883c9a233e79f16b59ec7aefb43d34d28c521
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162723"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationJob = await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"]
    .Request()
    .GetAsync();

```