---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91e67907ae428279d4c8960de4ed6f9268be3561
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509847"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = await graphClient.Oauth2permissiongrants["delta"]
    .Request()
    .GetAsync();

```