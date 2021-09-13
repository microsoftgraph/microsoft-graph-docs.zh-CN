---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ab3a8644d07c39403e01a700e664af2eb5641f769ba0511702c4ebb09d5c141
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409569"
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