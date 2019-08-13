---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fe2a916cef356c63bd96912b5661efaa36fb489e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327339"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailAppUsageUserCounts("D7")
    .buildRequest()
    .get();

```