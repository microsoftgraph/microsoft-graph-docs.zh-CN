---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c67e876b9fbc9422261cca1cd2b4b879a2ba1a4d1a770d815facc5b3d835e2fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215772"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableColumn workbookTableColumn = new WorkbookTableColumn();
workbookTableColumn.name = "name-value";
workbookTableColumn.index = 99;
workbookTableColumn.values = JsonParser.parseString("\"values-value\"");

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns("{id|name}")
    .buildRequest()
    .patch(workbookTableColumn);

```