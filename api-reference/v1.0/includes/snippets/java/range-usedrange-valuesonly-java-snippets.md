---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4f2ce1bbd9f20e4d9712bbcb02e3fb4dc9bf159
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980529"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .usedRange(WorkbookRangeUsedRangeParameterSet
        .newBuilder()
        .withValuesOnly(true)
        .build())
    .buildRequest()
    .get();

```