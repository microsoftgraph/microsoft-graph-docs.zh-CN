---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bc7b418a888f3ca737c90cee60f10cf3c0a4fbef
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359507"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessDeviceUsageDistributionUserCountsCollectionPage getSkypeForBusinessDeviceUsageDistributionUserCounts = graphClient.reports()
    .getSkypeForBusinessDeviceUsageDistributionUserCounts("D7")
    .buildRequest()
    .get();

```