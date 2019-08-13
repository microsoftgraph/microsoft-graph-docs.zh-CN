---
description: 自动生成的文件。 不修改
ms.openlocfilehash: aa0757b55bb2c19712007fda4e850d747e042fda
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320448"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getTeamsUserActivityCounts("D7")
    .buildRequest()
    .get();

```