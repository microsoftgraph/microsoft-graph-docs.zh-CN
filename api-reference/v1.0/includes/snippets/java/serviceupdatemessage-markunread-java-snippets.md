---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b688cdcef9dcd18538f517df7092c1d7d46494e3
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266757"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> messageIdsList = new LinkedList<String>();
messageIdsList.add("MC172851");
messageIdsList.add("MC167983");

graphClient.admin().serviceAnnouncement().messages()
    .markUnread(ServiceUpdateMessageMarkUnreadParameterSet
        .newBuilder()
        .withMessageIds(messageIdsList)
        .build())
    .buildRequest()
    .post();

```