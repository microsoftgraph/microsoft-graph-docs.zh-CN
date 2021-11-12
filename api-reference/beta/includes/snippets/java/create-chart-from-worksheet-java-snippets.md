---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 478529a72e05f1cbd541f989cb332143b5e07798336747f9c68d197c93954a8d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279452"
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