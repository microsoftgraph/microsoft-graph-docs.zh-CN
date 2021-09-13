---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92e11b7daf41b729eac3f6fd34e278a1fbfe0912916b7adc89c2fbcd8d5b1480
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105310"
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