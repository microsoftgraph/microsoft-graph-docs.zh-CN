---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bda33da833b5a851e2eaa80825c7a78ebc16a45c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338225"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var resourceActions = await graphClient.RoleManagement.Directory.ResourceNamespaces["{unifiedRbacResourceNamespace-id}"].ResourceActions
    .Request()
    .GetAsync();

```