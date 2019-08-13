---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7ab30618aac2b1377b1098fc7d54b79b7bb83719
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358517"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerDeviceUsageUserCountsCollectionPage getYammerDeviceUsageUserCounts = graphClient.reports()
    .getYammerDeviceUsageUserCounts("D7")
    .buildRequest()
    .get();

```