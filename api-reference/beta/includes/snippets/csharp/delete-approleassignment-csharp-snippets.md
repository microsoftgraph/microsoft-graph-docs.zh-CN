---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7abdb640a71db0a7f75261947064454f5fac40ef
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868321"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].AppRoleAssignedTo["{id}"]
    .Request()
    .DeleteAsync();

```