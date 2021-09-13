---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0a4ea7cdf0931d971a545d828b38cf8f9cf85eb8c1d1aa0025f275bace252dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219674"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartLineFormat workbookChartLineFormat = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().seriesAxis().format().line()
    .buildRequest()
    .get();

```