---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a2af24d838c1ce5045a2fd6bb0980f66f246337
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972066"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .createReply(MessageCreateReplyParameterSet
        .newBuilder()
        .withMessage(null)
        .withComment(null)
        .build())
    .buildRequest()
    .post();

```