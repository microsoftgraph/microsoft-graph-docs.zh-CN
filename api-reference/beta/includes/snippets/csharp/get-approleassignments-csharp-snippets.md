---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8803e13de770f6c692ef0da4cb605774cbc26ce0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499605"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignments = await graphClient.ServicePrincipals["{id}"].AppRoleAssignments
    .Request()
    .GetAsync();

```