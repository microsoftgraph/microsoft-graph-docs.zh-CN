---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e5d23c36084dfd1303cac313bb40f4ba9180722
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522806"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DirectoryRoles["{role-objectId}"].Members["{user-id}"].Reference
    .Request()
    .DeleteAsync();

```