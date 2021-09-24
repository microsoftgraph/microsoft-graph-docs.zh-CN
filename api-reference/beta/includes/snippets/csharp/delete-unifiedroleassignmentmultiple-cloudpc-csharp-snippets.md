---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3a649521ffed273287cd6b303bef309799ce40cf2284b50eee6f9640391ad63
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378361"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.RoleManagement.CloudPC.RoleAssignments["{unifiedRoleAssignmentMultiple-id}"]
    .Request()
    .DeleteAsync();

```