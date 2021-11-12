---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69a11bc5f0a3de5ee58c62443ed16ec0058d59f5875b8061ff9f30159ddcc440
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104461"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShare printerShare = new PrinterShare();
printerShare.displayName = "ShareName";
printerShare.allowAllUsers = false;
printerShare.additionalDataManager().put("printer@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/print/printers/{printerId}"));

graphClient.print().shares()
    .buildRequest()
    .post(printerShare);

```