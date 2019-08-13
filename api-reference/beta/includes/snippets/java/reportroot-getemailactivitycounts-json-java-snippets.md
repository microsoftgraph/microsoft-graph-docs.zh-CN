---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 865d9773719776441964194eee1694c9803d5614
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308803"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailActivitySummaryCollectionPage getEmailActivityCounts = graphClient.reports()
    .getEmailActivityCounts("D7")
    .buildRequest()
    .get();

```