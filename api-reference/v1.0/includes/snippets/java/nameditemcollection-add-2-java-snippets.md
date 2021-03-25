---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbb42a532c3c1a33ebaaf2b457a053b5acb8a159
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209847"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String name = "test7";

String formula = "=SUM(Sheet2!$A$1+Sheet2!$A$2)";

String comment = "Comment for the named item";

graphClient.me().drive().items("{id}").workbook().names()
    .addFormulaLocal(WorkbookNamedItemAddFormulaLocalParameterSet
        .newBuilder()
        .withName(name)
        .withFormula(formula)
        .withComment(comment)
        .build())
    .buildRequest()
    .post();

```