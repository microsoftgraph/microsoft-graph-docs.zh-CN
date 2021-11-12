---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9ce80988392f747bea3e88abc7e0e4ca9d9c3494ccd3fe8c46a8b0904f0d4cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56831184"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShare printerShare = new PrinterShare();
printerShare.displayName = "PrinterShare Name";
printerShare.additionalDataManager().put("printer@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/print/printers/{printerId}"));
printerShare.allowAllUsers = false;

graphClient.print().shares("{printerShareId}")
    .buildRequest()
    .patch(printerShare);

```