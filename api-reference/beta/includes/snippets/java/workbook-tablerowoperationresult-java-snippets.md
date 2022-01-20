---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39426950c94952934cfe8903035a0fa5b6c5b495
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136733"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableRow workbookTableRow = graphClient.me().drive().items("01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ").workbook()
    .tableRowOperationResult(WorkbookTableRowOperationResultParameterSet
        .newBuilder()
        .withKey("0195cfac-bd22-4f91-b276-dece0aa2378b")
        .build())
    .buildRequest()
    .get();

```