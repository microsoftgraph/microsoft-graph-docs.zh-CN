---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a45fd4fe16d6edc85f948b56276774e49da49ff8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949728"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String name = "test7";

String formula = "=SUM(Sheet2!$A$1+Sheet2!$A$2)";

String comment = "Comment for the named item";

graphClient.me().drive().items("{id}").workbook().names()
    .addFormulaLocal(name,formula,comment)
    .buildRequest()
    .post();

```