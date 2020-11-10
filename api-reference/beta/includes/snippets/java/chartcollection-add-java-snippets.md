---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf40bdbec9f62e5c0bd9a8dd84c745350ecb933d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958848"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "ColumnStacked";

JsonElement sourceData = JsonParser.parseString("A1:B1");

String seriesBy = "Auto";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts()
    .add(type,sourceData,seriesBy)
    .buildRequest()
    .post();

```