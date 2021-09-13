---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb80ac78040b56912dd2ed466265d0d80b54aad4cb0ba009014329ebc783be50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277502"
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