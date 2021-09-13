---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76f30943200bdeaac87d403d45228c16c0cd0052230193cfed13e21b439b5ba2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903893"
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