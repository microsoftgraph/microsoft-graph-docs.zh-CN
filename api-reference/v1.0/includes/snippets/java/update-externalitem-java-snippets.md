---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 085f49fb61ca47454ec6672c5f4936b956a66e45
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688747"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalItem externalItem = new ExternalItem();
LinkedList<Acl> aclList = new LinkedList<Acl>();
Acl acl = new Acl();
acl.type = AclType.EVERYONE;
acl.value = "67a141d8-cf4e-4528-ba07-bed21bfacd2d";
acl.accessType = AccessType.GRANT;
aclList.add(acl);
externalItem.acl = aclList;

graphClient.external().connections("contosohr").items("TSP228082938")
    .buildRequest()
    .patch(externalItem);

```