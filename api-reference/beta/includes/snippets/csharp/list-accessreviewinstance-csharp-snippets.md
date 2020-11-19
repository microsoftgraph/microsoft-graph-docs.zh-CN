---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 9f2fe5d70c3d75f484ae0131028b6a3dbe7d95f7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214722"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var instances = await graphClient.IdentityGovernance.AccessReviews.Definitions["60860cdd-fb4d-4054-91ba-f75e04f34444"].Instances
    .Request()
    .Skip(0)
    .Top(100)
    .GetAsync();

```