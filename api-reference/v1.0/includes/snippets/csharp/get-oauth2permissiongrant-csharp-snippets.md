---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75ba9bb9351ee144ef1fee342aaabc066dcd4193
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335382"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = await graphClient.Oauth2PermissionGrants["{id}"]
    .Request()
    .GetAsync();

```