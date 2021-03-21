---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9273dd7bc2c22929084ebd6165ec5928c0559c93
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983743"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookWorksheet workbookWorksheet = new WorkbookWorksheet();
workbookWorksheet.position = 99;
workbookWorksheet.name = "name-value";
workbookWorksheet.visibility = "visibility-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .buildRequest()
    .patch(workbookWorksheet);

```