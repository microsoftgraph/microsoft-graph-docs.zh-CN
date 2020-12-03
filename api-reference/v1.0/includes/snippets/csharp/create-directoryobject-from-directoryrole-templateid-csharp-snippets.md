---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c760e4f3aad7031fc17bee588bc80310d8bc36ca
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522649"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{user-id}"
};

await graphClient.DirectoryRoles["roleTemplateId={role-templateId}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```