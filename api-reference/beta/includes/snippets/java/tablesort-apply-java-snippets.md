---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e5ce2b4b26a8efc37997ab1668e5b16fa949ae4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978481"
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

String method = "method-value";

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").sort()
    .apply(WorkbookTableSortApplyParameterSet
        .newBuilder()
        .withFields(fieldsList)
        .withMatchCase(matchCase)
        .withMethod(method)
        .build())
    .buildRequest()
    .post();

```