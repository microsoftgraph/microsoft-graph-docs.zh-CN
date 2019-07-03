---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e8d5d291c4d97f513e04353f49e21b1d755a8f27
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499610"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = await graphClient.AppRoleAssignments["{id}"]
    .Request()
    .GetAsync();

```