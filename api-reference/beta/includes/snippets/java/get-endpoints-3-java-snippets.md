---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 816eac81e9b0d1db3e1196ee52b63d9c843f607b5328fb8ad9bb673e72a47c09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54274758"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinterCollectionPage dailyPrintUsageByPrinter = graphClient.print().reports().dailyPrintUsageByPrinter()
    .buildRequest()
    .get();

```