---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe736dbd321e1e9ac8ee6bb6588d3a7daa9b90f3
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51922627"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShare printerShare = new PrinterShare();
printerShare.displayName = "ShareName";
printerShare.allowAllUsers = true;
printerShare.additionalDataManager().put("printer@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/print/printers/{id}"));

graphClient.print().shares("{id}")
    .buildRequest()
    .patch(printerShare);

```