---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57b89224c3671faa7ca39bb73880997646c254fb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973576"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartAxis workbookChartAxis = new WorkbookChartAxis();
JsonElement majorUnit = new JsonObject();
workbookChartAxis.majorUnit = majorUnit;
JsonElement maximum = new JsonObject();
workbookChartAxis.maximum = maximum;
JsonElement minimum = new JsonObject();
workbookChartAxis.minimum = minimum;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().valueAxis()
    .buildRequest()
    .patch(workbookChartAxis);

```