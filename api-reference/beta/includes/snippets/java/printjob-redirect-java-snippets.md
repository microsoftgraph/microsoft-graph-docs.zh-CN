---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5730cc8c63a28ce27bb21aa224f5aeb0ec739bb8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970082"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String destinationPrinterId = "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea";

graphClient.print().printers("d5ef6ec4-07ca-4212-baf9-d45be126bfbb").jobs("44353")
    .redirect(PrintJobRedirectParameterSet
        .newBuilder()
        .withDestinationPrinterId(destinationPrinterId)
        .withConfiguration(null)
        .build())
    .buildRequest()
    .post();

```