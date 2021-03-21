---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5bc7a73814abf850fbd5402177d1eba9c9f3783
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972568"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .rowsAbove(WorkbookRangeRowsAboveParameterSet
        .newBuilder()
        .withCount(2)
        .build())
    .buildRequest()
    .get();

```