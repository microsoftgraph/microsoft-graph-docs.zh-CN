---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20285d7bc660f0528c892c501f8356f05704e7ff2587cf445f9b69e91944b366
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54274617"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByUserCollectionPage dailyPrintUsageByUser = graphClient.print().reports().dailyPrintUsageByUser()
    .buildRequest()
    .get();

```