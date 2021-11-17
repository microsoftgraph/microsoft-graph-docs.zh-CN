---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 578dc4b87ca4513dcacfcb2cccaffe3ebfaddcadb9dccef99031cb175dc5c98d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220197"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"]
    .Start()
    .Request()
    .PostAsync();

```