---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 086fdbfc0a3020b8912cd73e2bcd5c83ae278c538a7665dbde4e9614120081f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158405"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinterCollectionPage dailyPrintUsageByPrinter = graphClient.reports().dailyPrintUsageByPrinter()
    .buildRequest()
    .get();

```