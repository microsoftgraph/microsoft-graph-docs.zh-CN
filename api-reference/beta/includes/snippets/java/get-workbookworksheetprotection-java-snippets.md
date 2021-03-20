---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9741f3ae80ecc455321d311504b97bf7763293cd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969673"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookWorksheetProtection workbookWorksheetProtection = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").protection()
    .buildRequest()
    .get();

```