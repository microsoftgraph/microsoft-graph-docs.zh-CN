---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c65096fc594ff0dd9fd9d82c6788b2cb20a7e37e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971113"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String applyTo = "applyTo-value";

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .clear(WorkbookRangeClearParameterSet
        .newBuilder()
        .withApplyTo(applyTo)
        .build())
    .buildRequest()
    .post();

```