---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c817fa2bc5512fc667f5239d598c03254df3836
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522807"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DirectoryRoles["roleTemplateId={role-templateId}"].Members["{user-id}"].Reference
    .Request()
    .DeleteAsync();

```