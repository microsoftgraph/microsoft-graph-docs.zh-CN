---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35265e6b8877e1d75edcd594471170983d5197f7c689676ca8fdd85bb81185b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101307"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinterCollectionPage monthlyPrintUsageByPrinter = graphClient.reports().monthlyPrintUsageByPrinter()
    .buildRequest()
    .get();

```