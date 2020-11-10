---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ad1ef3facc3a89fb1abc99c9748b8941f95ebfc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958522"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartPoint workbookChartPoint = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series("{undefined}").points("{undefined}")
    .buildRequest()
    .get();

```