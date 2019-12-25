---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41d5b2a3e8b4bc7899bb8f80605d520798091b7f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868367"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = await graphClient.ServicePrincipals["{id}"].AppRoleAssignedTo["{id}"]
    .Request()
    .GetAsync();

```