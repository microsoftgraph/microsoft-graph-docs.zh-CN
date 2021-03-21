---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94b61c15a724edeecd6ab2a62376826c6d17cfc6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969642"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{id}").jobs("{id}")
    .abort(PrintJobAbortParameterSet
        .newBuilder()
        .withReason(null)
        .build())
    .buildRequest()
    .post();

```