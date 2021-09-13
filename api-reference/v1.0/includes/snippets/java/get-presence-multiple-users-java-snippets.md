---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbcac32438ce9ac2b480d806ab68c960b34bef63545d810c0575155ac1858fb4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903368"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> idsList = new LinkedList<String>();
idsList.add("fa8bf3dc-eca7-46b7-bad1-db199b62afc3");
idsList.add("66825e03-7ef5-42da-9069-724602c31f6b");

graphClient.communications()
    .getPresencesByUserId(CloudCommunicationsGetPresencesByUserIdParameterSet
        .newBuilder()
        .withIds(idsList)
        .build())
    .buildRequest()
    .post();

```