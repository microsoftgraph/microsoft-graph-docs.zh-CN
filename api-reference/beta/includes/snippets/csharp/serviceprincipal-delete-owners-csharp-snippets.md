---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 11c14dbaaaa281485c73c516047ee922dfd2fd41
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49350438"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].Owners["{id}"].Reference
    .Request()
    .DeleteAsync();

```