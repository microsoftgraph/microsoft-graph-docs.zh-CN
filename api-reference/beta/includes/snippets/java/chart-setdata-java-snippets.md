---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f4d18ef824fa24c5e289f1330fa038b47fd847b2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864275"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String sourceData = "sourceData-value";

String seriesBy = "seriesBy-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}")
    .setData(sourceData,seriesBy)
    .buildRequest()
    .post();

```