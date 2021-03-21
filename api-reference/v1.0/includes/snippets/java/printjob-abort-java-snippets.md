---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3287e6286621c8be40bd4b317e8b6d36f0ba0cb2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983112"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String reason = "String";

graphClient.print().printers("{printerId}").jobs("{printJobId}")
    .abort(PrintJobAbortParameterSet
        .newBuilder()
        .withReason(reason)
        .build())
    .buildRequest()
    .post();

```