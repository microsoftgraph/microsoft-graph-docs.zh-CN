---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 043cf1d1bd536246dfe3dd97e7c7ff80583795ff73accd904152bbc71af4d151
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333179"
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