---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e26b02a0eeee9546f4e110a206e55abf1a37ec6a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976378"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

Boolean sendResponse = true;

graphClient.me().events("{id}")
    .accept(EventAcceptParameterSet
        .newBuilder()
        .withComment(comment)
        .withSendResponse(sendResponse)
        .build())
    .buildRequest()
    .post();

```