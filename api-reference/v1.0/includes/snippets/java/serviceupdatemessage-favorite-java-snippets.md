---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4be3b2d37ca59e78e2ab44411ee6a50342554a67
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266656"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> messageIdsList = new LinkedList<String>();
messageIdsList.add("MC172851");
messageIdsList.add("MC167983");

graphClient.admin().serviceAnnouncement().messages()
    .favorite(ServiceUpdateMessageFavoriteParameterSet
        .newBuilder()
        .withMessageIds(messageIdsList)
        .build())
    .buildRequest()
    .post();

```