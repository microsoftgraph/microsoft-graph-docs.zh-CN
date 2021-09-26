---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c7acaf889d880fceec122fed677b81bb4b5f10e06e25d1c8a7d5be173f591ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164105"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = await graphClient.Oauth2PermissionGrants["{oAuth2PermissionGrant-id}"]
    .Request()
    .GetAsync();

```