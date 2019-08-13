---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8a3b6694de06d0d46269d7a69775d8fa23dc9f99
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360106"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOneDriveUsageAccountCountsCollectionPage getOneDriveUsageAccountCounts = graphClient.reports()
    .getOneDriveUsageAccountCounts("D7")
    .buildRequest()
    .get();

```