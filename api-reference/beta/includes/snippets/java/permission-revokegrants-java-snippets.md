---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c4868098797e584ca55e1b52e428ede9c9cfcd0bf60d1b709ab87009aaedd77
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220265"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<DriveRecipient> granteesList = new LinkedList<DriveRecipient>();
DriveRecipient grantees = new DriveRecipient();
grantees.email = "ryan@contoso.com";

granteesList.add(grantees);

graphClient.me().drive().items("{item-id}").permissions("{perm-id}")
    .revokeGrants(PermissionRevokeGrantsParameterSet
        .newBuilder()
        .withGrantees(granteesList)
        .build())
    .buildRequest()
    .post();

```