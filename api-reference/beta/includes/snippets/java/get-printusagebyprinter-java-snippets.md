---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2198f2f262b278940ab638500bc71fe58a91a63924b1c89e5d05d4a7ef26058b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221081"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinter printUsageByPrinter = graphClient.print().reports().dailyPrintUsageByPrinter("016b5565-3bbf-4067-b9ff-4d68167eb1a6")
    .buildRequest()
    .get();

```