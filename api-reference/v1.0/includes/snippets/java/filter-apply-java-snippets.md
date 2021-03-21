---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d13685b40d44ca9562552f33baa4aa259e9582c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966671"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
JsonElement values = new JsonObject();
criteria.values = values;
criteria.filterOn = "filterOn-value";

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns("{id|name}").filter()
    .apply(WorkbookFilterApplyParameterSet
        .newBuilder()
        .withCriteria(criteria)
        .build())
    .buildRequest()
    .post();

```