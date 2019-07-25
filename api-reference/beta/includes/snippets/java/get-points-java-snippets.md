---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c9a418d938a988781c25dc8b45cf953e0f38475d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863770"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookChartPointCollectionPage points = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series("{undefined}").points()
    .buildRequest()
    .get();

```