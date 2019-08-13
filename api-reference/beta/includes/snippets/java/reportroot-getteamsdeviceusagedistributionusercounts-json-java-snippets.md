---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3f52e60fa339cf53db1911eee7895a0c429a732b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358872"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsDeviceUsageDistributionUserCountsCollectionPage getTeamsDeviceUsageDistributionUserCounts = graphClient.reports()
    .getTeamsDeviceUsageDistributionUserCounts("D7")
    .buildRequest()
    .get();

```