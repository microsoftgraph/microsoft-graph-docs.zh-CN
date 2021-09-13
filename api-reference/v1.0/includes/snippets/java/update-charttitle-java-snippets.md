---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 626f83a0eff5f600c0d9149cd18ed8b9e0ad52ba82505169748fedeb4b472782
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378457"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartTitle workbookChartTitle = new WorkbookChartTitle();
workbookChartTitle.overlay = true;
workbookChartTitle.text = "text-value";
workbookChartTitle.visible = true;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").title()
    .buildRequest()
    .patch(workbookChartTitle);

```