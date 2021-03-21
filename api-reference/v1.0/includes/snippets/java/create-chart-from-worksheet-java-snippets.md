---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4afc1c0fc0bd6ef38fc84ced096540c8dfb27577
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980458"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChart workbookChart = new WorkbookChart();
workbookChart.id = "id-value";
workbookChart.height = 99d;
workbookChart.left = 99d;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts()
    .buildRequest()
    .post(workbookChart);

```