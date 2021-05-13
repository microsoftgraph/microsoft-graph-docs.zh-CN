---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88e680c3cdbb184bc62b9f2bcb23a94b54f7ab84
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474681"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleSchedules = await graphClient.RoleManagement.Directory
    .RoleSchedules("a3bb8764-cb92-4276-9d2a-ca1e895e55ea","a3bb8764-cb92-4276-9d2a-ca1e895e55ea","a3bb8764-cb92-4276-9d2a-ca1e895e55ea","a3bb8764-cb92-4276-9d2a-ca1e895e55ea")
    .Request()
    .GetAsync();

```