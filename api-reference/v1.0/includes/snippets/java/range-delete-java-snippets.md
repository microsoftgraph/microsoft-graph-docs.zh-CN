---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bfca346e06694ec5cc9074c64bb2b75483b0c3f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974202"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String shift = "shift-value";

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .delete(WorkbookRangeDeleteParameterSet
        .newBuilder()
        .withShift(shift)
        .build())
    .buildRequest()
    .post();

```