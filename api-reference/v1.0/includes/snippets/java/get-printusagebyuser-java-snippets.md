---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30a18d7861aca5cc4bffe7594c0b81043c745d0b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972077"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByUser printUsageByUser = graphClient.reports().dailyPrintUsageByUser("{id}")
    .buildRequest()
    .get();

```