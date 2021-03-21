---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4057365ffec698670ed848681232cf182f649d7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978241"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .columnsAfter(WorkbookRangeColumnsAfterParameterSet
        .newBuilder()
        .withCount(2)
        .build())
    .buildRequest()
    .get();

```