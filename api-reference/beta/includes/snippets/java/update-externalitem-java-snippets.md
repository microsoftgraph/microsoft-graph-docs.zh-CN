---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6c475391ba9be4fa3b91145576ebe352bbe298d
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694518"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalItem externalItem = new ExternalItem();
LinkedList<Acl> aclList = new LinkedList<Acl>();
Acl acl = new Acl();
acl.type = AclType.EVERYONE;
acl.value = "67a141d8-cf4e-4528-ba07-bed21bfacd2d";
acl.accessType = AccessType.GRANT;
acl.identitySource = IdentitySourceType.AZURE_ACTIVE_DIRECTORY;
aclList.add(acl);
externalItem.acl = aclList;

graphClient.external().connections("contosohr").items("TSP228082938")
    .buildRequest()
    .patch(externalItem);

```