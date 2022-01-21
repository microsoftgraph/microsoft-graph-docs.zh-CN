---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99ff4aa58266fbbce3dca3e94d1dee82f96ca6382754c966c6f8915c9c27fb4a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218868"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var functions = await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"].Schema
    .Functions()
    .Request()
    .GetAsync();

```