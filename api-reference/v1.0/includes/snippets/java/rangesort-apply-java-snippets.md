---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f899d5edcd7b84f2d28728e02caf4cbde6c991d888bca11cadee830d610ce910
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104457"
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