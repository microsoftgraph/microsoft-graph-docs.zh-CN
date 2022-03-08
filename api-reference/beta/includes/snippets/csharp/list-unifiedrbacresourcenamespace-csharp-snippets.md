---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d54a4a8216fa50b77933d92191957dda2797c65b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338382"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var resourceNamespaces = await graphClient.RoleManagement.Directory.ResourceNamespaces
    .Request()
    .GetAsync();

```