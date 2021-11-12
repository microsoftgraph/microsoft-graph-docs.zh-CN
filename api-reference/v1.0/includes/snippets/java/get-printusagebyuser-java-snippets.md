---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2607a09468cac92dc074201308c252bbc42c25b54033b045fd0cfef85f090baa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104940"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByUser printUsageByUser = graphClient.reports().dailyPrintUsageByUser("{id}")
    .buildRequest()
    .get();

```