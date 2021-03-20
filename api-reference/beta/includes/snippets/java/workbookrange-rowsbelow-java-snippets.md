---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f37fd7b818ce0ad80b8b3becf3ac49e377ca09b3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966988"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .rowsBelow(WorkbookRangeRowsBelowParameterSet
        .newBuilder()
        .withCount(2)
        .build())
    .buildRequest()
    .get();

```