---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1434cb389bd20624d1116cee7673cd2c03975ab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973215"
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