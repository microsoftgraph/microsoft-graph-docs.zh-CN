---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01913f6be82426c748882113207e4df64a769cd3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967135"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RejectReason reason = RejectReason.BUSY;

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .reject(CallRejectParameterSet
        .newBuilder()
        .withReason(reason)
        .withCallbackUri(null)
        .build())
    .buildRequest()
    .post();

```