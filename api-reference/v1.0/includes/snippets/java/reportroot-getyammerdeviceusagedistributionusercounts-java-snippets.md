---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b6555e18190accc7eeaa9a625225e3d64d38908c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320309"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerDeviceUsageDistributionUserCounts("D7")
    .buildRequest()
    .get();

```