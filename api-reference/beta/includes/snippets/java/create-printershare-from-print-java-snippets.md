---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a539ef4f171a6739ca7a627f562c73d816e7fd140b960f3ed5a8b22b4b2e061
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903312"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShare printerShare = new PrinterShare();
printerShare.name = "name-value";
printerShare.additionalDataManager().put("printer@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/print/printers/{id}"));

graphClient.print().shares()
    .buildRequest()
    .post(printerShare);

```