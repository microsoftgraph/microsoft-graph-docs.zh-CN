---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 988e5bd0e439e88343246bc6173863ee4f827e6d
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869011"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.CloudPC.RoleAssignments
    .Request()
    .Filter("roleDefinitionId eq 'b5c08161-a7af-481c-ace2-a20a69a48fb1'")
    .GetAsync();

```