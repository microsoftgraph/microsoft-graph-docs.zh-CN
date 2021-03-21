---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c03d00fdad3f5fcacd894c2867027fe8d81dd61c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977536"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .rowsAbove(WorkbookRangeRowsAboveParameterSet
        .newBuilder()
        .withCount(2)
        .build())
    .buildRequest()
    .get();

```