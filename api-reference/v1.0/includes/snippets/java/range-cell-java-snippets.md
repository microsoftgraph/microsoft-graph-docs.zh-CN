---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f02f8ba360f029dad65a09270c550755971465b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979800"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .cell(WorkbookRangeCellParameterSet
        .newBuilder()
        .withRow(5)
        .withColumn(6)
        .build())
    .buildRequest()
    .get();

```