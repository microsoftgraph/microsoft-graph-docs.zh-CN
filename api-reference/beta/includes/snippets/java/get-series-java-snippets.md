---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70895642ac1c2e4d82074602ec5b70036e85f15f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959059"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookChartSeriesCollectionPage series = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series()
    .buildRequest()
    .get();

```