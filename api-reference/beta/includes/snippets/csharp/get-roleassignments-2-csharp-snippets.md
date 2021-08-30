---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93e74bfb71a20a4b27d680346395e9db22e2335c320e6c41c43b7b32b5aab1ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378395"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.Directory.RoleAssignments
    .Request()
    .GetAsync();

```