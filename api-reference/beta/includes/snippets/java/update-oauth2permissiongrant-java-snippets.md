---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2dd65c280546d8dcad171d2efaa3d4273f7b955a
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758651"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrant oAuth2PermissionGrant = new OAuth2PermissionGrant();
oAuth2PermissionGrant.scope = "User.ReadBasic.All Group.ReadWrite.All";

graphClient.oauth2PermissionGrants("l5eW7x0ga0-WDOntXzHateQDNpSH5-lPk9HjD3Sarjk")
    .buildRequest()
    .patch(oAuth2PermissionGrant);

```