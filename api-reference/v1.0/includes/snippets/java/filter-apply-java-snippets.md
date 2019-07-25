---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b597475bfa8a3983accfc826f0543447da19e870
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885535"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookFilterCriteria criteria = new WorkbookFilterCriteria();
criteria.criterion1 = "criterion1-value";
criteria.criterion2 = "criterion2-value";
criteria.color = "color-value";
String operator = new String();
criteria.operator = operator;
WorkbookIcon icon = new WorkbookIcon();
icon.set = "set-value";
icon.index = 99;
criteria.icon = icon;
criteria.dynamicCriteria = "dynamicCriteria-value";
Json values = new Json();
criteria.values = values;
criteria.filterOn = "filterOn-value";

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns("{id|name}").filter()
    .apply(criteria)
    .buildRequest()
    .post();

```