---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43f7cc27ef65daa02aa9388d5a17b8d3b71a7107a9854b1715c15e01f25e5771
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278910"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.CloudPC.RoleAssignments
    .Request()
    .Filter("roleDefinitionId eq 'b5c08161-a7af-481c-ace2-a20a69a48fb1'")
    .GetAsync();

```