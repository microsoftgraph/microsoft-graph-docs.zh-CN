---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f52ccacd5b5b38f8670979f76169e3ee8c89b74
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982861"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Permission permission = new Permission();
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("write");
permission.roles = rolesList;
LinkedList<IdentitySet> grantedToIdentitiesList = new LinkedList<IdentitySet>();
IdentitySet grantedToIdentities = new IdentitySet();
Identity application = new Identity();
application.id = "89ea5c94-7736-4e25-95ad-3fa95f62b66e";
application.displayName = "Foo App";
grantedToIdentities.application = application;
grantedToIdentitiesList.add(grantedToIdentities);
permission.grantedToIdentities = grantedToIdentitiesList;

graphClient.sites("{sitesId}").permissions()
    .buildRequest()
    .post(permission);

```