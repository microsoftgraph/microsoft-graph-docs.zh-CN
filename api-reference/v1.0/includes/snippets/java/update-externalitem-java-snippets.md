---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f171a90a9234ac7ae7fc0f80b628dd37e3d78f2d1ddceedc9297ea273f9a2043
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279358"
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

graphClient.connections("contosohr").items("TSP228082938")
    .buildRequest()
    .patch(externalItem);

```