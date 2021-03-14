---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 063b88365e5fec0bccf9c9fc8008a198966b4542
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789977"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Oauth2PermissionGrants["{oAuth2PermissionGrant-id}"]
    .Request()
    .DeleteAsync();

```