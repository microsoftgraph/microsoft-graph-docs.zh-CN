---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d2c2353d2ebc6ec9182d379e9eac4a4a3b5493d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954815"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintUsageByUserCollectionPage dailyPrintUsageByUser = graphClient.reports().dailyPrintUsageByUser()
    .buildRequest()
    .get();

```