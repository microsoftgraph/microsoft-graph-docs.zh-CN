---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d144c3f48bca345416fee8ecaf692e01c663faa2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972035"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .columnsAfter(WorkbookRangeColumnsAfterParameterSet
        .newBuilder()
        .withCount(2)
        .build())
    .buildRequest()
    .get();

```