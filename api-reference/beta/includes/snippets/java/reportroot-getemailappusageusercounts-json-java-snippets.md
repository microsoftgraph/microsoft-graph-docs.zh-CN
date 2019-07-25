---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 48601837f506ca419fc9f857f2ee66403d323855
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873891"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAppUsageUserCountsCollectionPage getEmailAppUsageUserCounts = graphClient.reports()
    .getEmailAppUsageUserCounts('D7')
    .buildRequest()
    .get();

```