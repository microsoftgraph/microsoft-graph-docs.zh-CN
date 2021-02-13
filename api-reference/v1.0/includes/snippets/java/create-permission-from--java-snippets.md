---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e1cef7b7979d71e556a84461720a0b83ce3e627
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176770"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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