---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fd25931e143ae51472f64ab1b706c6ac39095697
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327284"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailAppUsageVersionsUserCounts("D7")
    .buildRequest()
    .get();

```