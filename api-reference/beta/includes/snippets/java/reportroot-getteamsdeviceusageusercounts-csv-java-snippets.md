---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 55199617365bd14eb7e6ece14c09b8b1635713d2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358884"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsDeviceUsageUserCountsCollectionPage getTeamsDeviceUsageUserCounts = graphClient.reports()
    .getTeamsDeviceUsageUserCounts("D7")
    .buildRequest()
    .get();

```