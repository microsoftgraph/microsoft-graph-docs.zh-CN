---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a758d7ee582d3c53da6fac81a648297099283ac6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971803"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("A1:Z10")
        .build())
    .visibleView()
    .range()
    .buildRequest()
    .get();

```