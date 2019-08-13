---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f7d872fdb726eb8758594a92d99c450ece8dae28
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320280"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerDeviceUsageUserCounts("D7")
    .buildRequest()
    .get();

```