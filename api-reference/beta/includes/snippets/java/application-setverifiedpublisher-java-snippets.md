---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbc5090471a97845c913424c8eb4bb198162dc5d
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53578866"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String verifiedPublisherId = "1234567";

graphClient.applications("{id}")
    .setVerifiedPublisher(ApplicationSetVerifiedPublisherParameterSet
        .newBuilder()
        .withVerifiedPublisherId(verifiedPublisherId)
        .build())
    .buildRequest()
    .post();

```