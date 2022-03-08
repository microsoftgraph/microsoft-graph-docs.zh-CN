---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2058ad6d572fb061dca6b08f381d6a549a077bcb
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338282"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRbacResourceAction = await graphClient.RoleManagement.Directory.ResourceNamespaces["{unifiedRbacResourceNamespace-id}"].ResourceActions["{unifiedRbacResourceAction-id}"]
    .Request()
    .GetAsync();

```