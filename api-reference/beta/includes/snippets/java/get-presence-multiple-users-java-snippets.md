---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c3a73c93246eab011be77f6e23a143eb7c460fc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977175"
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