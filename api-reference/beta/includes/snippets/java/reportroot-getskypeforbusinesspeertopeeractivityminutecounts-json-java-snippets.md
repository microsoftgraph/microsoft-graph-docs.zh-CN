---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e05c397c53bd30d77f9f3f76230fd34c51f7ed26
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358981"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessPeerToPeerActivityMinuteCountsCollectionPage getSkypeForBusinessPeerToPeerActivityMinuteCounts = graphClient.reports()
    .getSkypeForBusinessPeerToPeerActivityMinuteCounts("D7")
    .buildRequest()
    .get();

```