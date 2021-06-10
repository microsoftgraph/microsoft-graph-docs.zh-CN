---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6aa928f66da36ee1372b10e8bccb644c2b720db1
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871394"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByUserCollectionPage monthlyPrintUsageByUser = graphClient.print().reports().monthlyPrintUsageByUser()
    .buildRequest()
    .get();

```