---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e262e1f9f20d293d8fca9bcb8c6d7414f069246
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973109"
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