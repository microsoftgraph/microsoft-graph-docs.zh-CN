---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 03bf14dcc2f511af58020ff1cfb89d9c0b08cbe9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888017"
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

String method = "method-value";

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").sort()
    .apply(fieldsList,matchCase,method)
    .buildRequest()
    .post();

```