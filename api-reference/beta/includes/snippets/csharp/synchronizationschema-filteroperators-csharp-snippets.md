---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e0c545a8c6d88881c1ed0284391a9139a4d779b65944ccbed4fe1a43513b747
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161375"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterOperators = await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"].Schema
    .FilterOperators()
    .Request()
    .GetAsync();

```