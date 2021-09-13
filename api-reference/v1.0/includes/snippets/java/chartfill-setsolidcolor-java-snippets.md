---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07f21466489afbdde6b23407f5b4e110c04faa5d2478c5ea960435b2f7cdb86d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333996"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String color = "color-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").format().fill()
    .setSolidColor(WorkbookChartFillSetSolidColorParameterSet
        .newBuilder()
        .withColor(color)
        .build())
    .buildRequest()
    .post();

```