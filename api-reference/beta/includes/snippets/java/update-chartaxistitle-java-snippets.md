---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c9baac68eeadfb8df4af0a522452fe875331c82fdf4315b886f71c463c19cb2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104891"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartAxisTitle workbookChartAxisTitle = new WorkbookChartAxisTitle();
workbookChartAxisTitle.text = "text-value";
workbookChartAxisTitle.visible = true;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().valueAxis().title()
    .buildRequest()
    .patch(workbookChartAxisTitle);

```