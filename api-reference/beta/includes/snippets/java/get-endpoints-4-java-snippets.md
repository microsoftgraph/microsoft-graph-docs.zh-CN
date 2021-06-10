---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd8c399519a02f2e3172ad7c714f4198c915e015
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871526"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByUserCollectionPage dailyPrintUsageByUser = graphClient.print().reports().dailyPrintUsageByUser()
    .buildRequest()
    .get();

```