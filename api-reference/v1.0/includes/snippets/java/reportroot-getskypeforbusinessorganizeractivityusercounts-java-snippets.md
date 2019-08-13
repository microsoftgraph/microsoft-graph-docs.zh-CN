---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0d3fe05d404a4bd3b7385e82faa0db1af0cc7f2e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320730"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessOrganizerActivityUserCounts("D7")
    .buildRequest()
    .get();

```