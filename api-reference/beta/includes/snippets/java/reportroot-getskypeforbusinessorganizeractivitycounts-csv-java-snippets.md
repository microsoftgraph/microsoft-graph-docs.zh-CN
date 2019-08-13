---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 728c8eb55100efe270283caae0bd08213d6355b6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359338"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessOrganizerActivityCountsCollectionPage getSkypeForBusinessOrganizerActivityCounts = graphClient.reports()
    .getSkypeForBusinessOrganizerActivityCounts("D7")
    .buildRequest()
    .get();

```