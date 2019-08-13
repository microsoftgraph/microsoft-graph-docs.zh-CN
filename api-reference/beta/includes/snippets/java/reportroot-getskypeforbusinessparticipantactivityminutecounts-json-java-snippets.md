---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4f08d889caef1c936714229d3e39a542c195c2e5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359132"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessParticipantActivityMinuteCountsCollectionPage getSkypeForBusinessParticipantActivityMinuteCounts = graphClient.reports()
    .getSkypeForBusinessParticipantActivityMinuteCounts("D7")
    .buildRequest()
    .get();

```