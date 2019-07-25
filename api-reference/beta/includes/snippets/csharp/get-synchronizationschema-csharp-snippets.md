---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 029f568395f4db3997956bc93746c39ab5ba7ea2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715419"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationSchema = await graphClient.ServicePrincipals["{servicePrincipalId}"].Synchronization.Jobs["{jobId}"].Schema
    .Request()
    .Header("Authorization","Bearer {Token}")
    .GetAsync();

```