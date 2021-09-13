---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6a460433a1737e605c164c2b5f008bf203419c16096f50f41de59c8f6cf6673
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334107"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

graphClient.me().messages("{id}")
    .replyAll(MessageReplyAllParameterSet
        .newBuilder()
        .withMessage(null)
        .withComment(comment)
        .build())
    .buildRequest()
    .post();

```