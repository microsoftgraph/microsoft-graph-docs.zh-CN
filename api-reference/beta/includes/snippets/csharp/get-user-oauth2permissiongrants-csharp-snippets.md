---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37a3f06d07813207042d750aac57567a7b8b8a64
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332552"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oauth2PermissionGrants = await graphClient.Users["{id}"].Oauth2PermissionGrants
    .Request()
    .GetAsync();

```