---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7947e8c4addf5113382d484e0b43d48211f5662a0fd37fe220b492781419c48c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219003"
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