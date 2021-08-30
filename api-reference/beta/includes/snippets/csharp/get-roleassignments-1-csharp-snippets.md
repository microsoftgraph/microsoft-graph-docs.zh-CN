---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba451a902b07cd0d0fb29cd33c3afe40b7c9914b58deaf81e2523b660b81358f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378394"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.Directory.RoleAssignments
    .Request()
    .Filter("roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'")
    .Expand("principal")
    .GetAsync();

```