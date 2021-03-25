---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d87e2e7cf9ca704054d25065941d497f0ced64dd
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208867"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByUserCollectionPage monthlyPrintUsageSummariesByUser = graphClient.print().reports().monthlyPrintUsageSummariesByUser()
    .buildRequest()
    .get();

```