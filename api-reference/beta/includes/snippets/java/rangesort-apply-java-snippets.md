---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0d35fe1c4e59c4747c018a7510a24739201a9d86
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874184"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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

boolean matchCase = True;

boolean hasHeaders = True;

String orientation = "orientation-value";

String method = "method-value";

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().sort()
    .apply(fieldsList,matchCase,hasHeaders,orientation,method)
    .buildRequest()
    .post();

```