---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1fe05a6605eacb7d24573028d17cfaafb80055c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573165"
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
application.displayName = "Contoso Time Manager App";
grantedToIdentities.application = application;
grantedToIdentitiesList.add(grantedToIdentities);
permission.grantedToIdentities = grantedToIdentitiesList;

graphClient.sites("{sitesId}").permissions()
    .buildRequest()
    .post(permission);

```