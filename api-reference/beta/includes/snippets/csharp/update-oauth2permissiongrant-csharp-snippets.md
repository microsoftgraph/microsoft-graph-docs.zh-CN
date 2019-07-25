---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 83706e6c53bf56778ff6b9f9a37a635577d4ef15
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721160"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = new OAuth2PermissionGrant
{
    Scope = "scope-value"
};

await graphClient.OAuth2Permissiongrants["{id}"]
    .Request()
    .UpdateAsync(oAuth2PermissionGrant);

```