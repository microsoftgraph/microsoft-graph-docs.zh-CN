---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 70e337dc1ebd384bbfa65eb1f71609d303286a2b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359849"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365ActiveUserCountsCollectionPage getOffice365ActiveUserCounts = graphClient.reports()
    .getOffice365ActiveUserCounts("D7")
    .buildRequest()
    .get();

```