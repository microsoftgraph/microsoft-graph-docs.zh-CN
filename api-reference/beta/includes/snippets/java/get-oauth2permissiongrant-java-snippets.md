---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6cfb6cf359f8c21b41ed3aecb568637f9e529b7f4f5f8d1ccb46bbb5c2f952e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277602"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrant oAuth2PermissionGrant = graphClient.oauth2PermissionGrants("{id}")
    .buildRequest()
    .get();

```