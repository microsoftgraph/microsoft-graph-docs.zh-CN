---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5db1a2d87c5e742df359abc7bfeaa0aeb62ae032
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981536"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<WorkbookSortField> fieldsList = new LinkedList<WorkbookSortField>();
WorkbookSortField fields = new WorkbookSortField();
fields.key = 99;
fields.sortOn = "sortOn-value";
fields.ascending = true;
fields.color = "color-value";
fields.dataOption = "dataOption-value";
WorkbookIcon icon = new WorkbookIcon();
icon.set = "set-value";
icon.index = 99;
fields.icon = icon;

fieldsList.add(fields);

Boolean matchCase = true;

Boolean hasHeaders = true;

String orientation = "orientation-value";

String method = "method-value";

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().sort()
    .apply(WorkbookRangeSortApplyParameterSet
        .newBuilder()
        .withFields(fieldsList)
        .withMatchCase(matchCase)
        .withHasHeaders(hasHeaders)
        .withOrientation(orientation)
        .withMethod(method)
        .build())
    .buildRequest()
    .post();

```