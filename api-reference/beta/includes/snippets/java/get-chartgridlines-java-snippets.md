---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0892fa00e597b7f8837ceaf7284ba27d98d20bee
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958681"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartGridlines workbookChartGridlines = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().valueAxis().minorGridlines()
    .buildRequest()
    .get();

```