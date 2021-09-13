---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b9b182cf94cf8906ceb7686630c5b610a2b1267
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59097852"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignment = await graphClient.RoleManagement.Directory.RoleAssignments["{unifiedRoleAssignment-id}"]
    .Request()
    .Expand("directoryScope")
    .GetAsync();

```