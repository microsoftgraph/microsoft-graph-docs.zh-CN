---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 274ac792f2e3329f7e78acc06d89ec5a48856e0e4796932bf70cf8f5857152a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164114"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookFormatProtection workbookFormatProtection = new WorkbookFormatProtection();
workbookFormatProtection.locked = true;
workbookFormatProtection.formulaHidden = true;

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().protection()
    .buildRequest()
    .patch(workbookFormatProtection);

```