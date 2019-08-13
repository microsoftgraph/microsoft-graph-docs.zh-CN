---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 008947e82ffb4f902cb397aca9de8404550102ee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359173"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessParticipantActivityCountsCollectionPage getSkypeForBusinessParticipantActivityCounts = graphClient.reports()
    .getSkypeForBusinessParticipantActivityCounts("D7")
    .buildRequest()
    .get();

```