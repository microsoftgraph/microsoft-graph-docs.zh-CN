---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 30e73bc4e98a181922e013d5b469b54ddad69206
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871889"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessPeerToPeerActivityUserCountsCollectionPage getSkypeForBusinessPeerToPeerActivityUserCounts = graphClient.reports()
    .getSkypeForBusinessPeerToPeerActivityUserCounts('D7')
    .buildRequest()
    .get();

```