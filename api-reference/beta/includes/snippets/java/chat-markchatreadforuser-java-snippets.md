---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9219c63e43873d4c841a4df2bc47d9a917b10a6
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890650"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkUserIdentity user = new TeamworkUserIdentity();
user.id = "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2";

String tenantId = "2a690434-97d9-4eed-83a6-f5f13600199a";

graphClient.chats("19:7d898072-792c-4006-bb10-5ca9f2590649_8ea0e38b-efb3-4757-924a-5f94061cf8c2@unq.gbl.spaces")
    .markChatReadForUser(ChatMarkChatReadForUserParameterSet
        .newBuilder()
        .withUser(user)
        .withTenantId(tenantId)
        .build())
    .buildRequest()
    .post();

```