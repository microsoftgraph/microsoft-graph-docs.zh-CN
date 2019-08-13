---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fece4c56bc83434a8ea31bfac145d45f5b7862b0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327368"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailAppUsageAppsUserCounts("D7")
    .buildRequest()
    .get();

```