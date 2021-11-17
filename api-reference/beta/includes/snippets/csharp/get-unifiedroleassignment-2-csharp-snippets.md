---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 310994a9cf7a82f94b30cf5ef8cbc445f8a2071cc0d6998eb18c2587245bf0ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904005"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignment = await graphClient.RoleManagement.Directory.RoleAssignments["{unifiedRoleAssignment-id}"]
    .Request()
    .Expand("directoryScope")
    .GetAsync();

```