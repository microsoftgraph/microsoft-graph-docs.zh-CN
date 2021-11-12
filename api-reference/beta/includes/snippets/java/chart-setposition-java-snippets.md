---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 581b9f747db73a106d92e1a887cb5f0e04b4a1c3ece76e3773f5f1518ca49762
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378298"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

JsonElement startCell = JsonParser.parseString("startCell-value");

JsonElement endCell = JsonParser.parseString("endCell-value");

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}")
    .setPosition(WorkbookChartSetPositionParameterSet
        .newBuilder()
        .withStartCell(startCell)
        .withEndCell(endCell)
        .build())
    .buildRequest()
    .post();

```