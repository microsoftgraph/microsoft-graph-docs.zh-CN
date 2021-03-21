---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96f1486a3e6786c2ac5b34b6448f473f63d46160
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983835"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean across = true;

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .merge(WorkbookRangeMergeParameterSet
        .newBuilder()
        .withAcross(across)
        .build())
    .buildRequest()
    .post();

```