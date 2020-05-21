---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd4e62e16696cfdc718b1a41a0f8c28e1ee2f1ef
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335294"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oauth2PermissionGrants = await graphClient.Oauth2PermissionGrants
    .Request()
    .GetAsync();

```