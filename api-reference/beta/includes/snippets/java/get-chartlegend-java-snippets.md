---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ed604542baad909cd11971f0cfd1e9fe2963426e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863925"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartLegend workbookChartLegend = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").legend()
    .buildRequest()
    .get();

```