---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a1492de53f7907a8b85677838930914cf609a082
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360679"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAppUsageVersionsUserCountsCollectionPage getEmailAppUsageVersionsUserCounts = graphClient.reports()
    .getEmailAppUsageVersionsUserCounts("D7")
    .buildRequest()
    .get();

```