---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f091cf9f12b23bf4ca34a5d764b349142a56951e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320478"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getTeamsDeviceUsageUserDetail("D7")
    .buildRequest()
    .get();

```