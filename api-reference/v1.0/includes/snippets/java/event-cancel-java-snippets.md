---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6b5f2171f1121a89c30ee22eebc6008fb05d5e0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976322"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "Cancelling for this week due to all hands";

graphClient.me().events("{id}")
    .cancel(EventCancelParameterSet
        .newBuilder()
        .withComment(comment)
        .build())
    .buildRequest()
    .post();

```