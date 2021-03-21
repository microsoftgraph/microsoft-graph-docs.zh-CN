---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f0449799d9184a7d380c281b478b1cb0fee308e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974979"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .createForward(MessageCreateForwardParameterSet
        .newBuilder()
        .withToRecipients(null)
        .withMessage(null)
        .withComment(null)
        .build())
    .buildRequest()
    .post();

```