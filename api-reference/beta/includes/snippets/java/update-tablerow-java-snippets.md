---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 12a92c7c4e0c7cc57b36d02455c2e1d8e1d41c63
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868503"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableRow workbookTableRow = new WorkbookTableRow();
workbookTableRow.index = 99;
workbookTableRow.values = "values-value";

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").rows("{index}")
    .buildRequest()
    .patch(workbookTableRow);

```