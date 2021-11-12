---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 544b695fa220a2a9c8201d2df7b146b7a145589c28d4661b521d60b746e04bd9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106460"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartLineFormat workbookChartLineFormat = new WorkbookChartLineFormat();
workbookChartLineFormat.color = "color-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().seriesAxis().format().line()
    .buildRequest()
    .patch(workbookChartLineFormat);

```