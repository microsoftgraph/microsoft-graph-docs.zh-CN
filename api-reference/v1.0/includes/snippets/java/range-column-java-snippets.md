---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 957512144ef3f54fe88d9212ee7554321b5eb91fbbc6c2f680fd07f79c9cf615
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104564"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .column(WorkbookRangeColumnParameterSet
        .newBuilder()
        .withColumn(5)
        .build())
    .buildRequest()
    .get();

```