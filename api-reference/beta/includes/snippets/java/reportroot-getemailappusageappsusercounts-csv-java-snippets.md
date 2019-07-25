---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c242920478679fb438d0308350d7a98fe6fe229f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873934"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAppUsageAppsUserCountsCollectionPage getEmailAppUsageAppsUserCounts = graphClient.reports()
    .getEmailAppUsageAppsUserCounts('D7')
    .buildRequest()
    .get();

```