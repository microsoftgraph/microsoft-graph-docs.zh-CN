---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 83706e6c53bf56778ff6b9f9a37a635577d4ef15
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479855"
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