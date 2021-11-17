---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c08da343e6a74796823529eac81e810e71a8c8ce8d829dc22e0ba1e643850348
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332453"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationSchema = await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"].Schema
    .Request()
    .Header("Authorization","Bearer {Token}")
    .GetAsync();

```