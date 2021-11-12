---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef388e8b19aeb88693cd47075879c068f29f52bd636939aa10dc89ee937d4fd0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902459"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookWorksheetProtection workbookWorksheetProtection = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").protection()
    .buildRequest()
    .get();

```