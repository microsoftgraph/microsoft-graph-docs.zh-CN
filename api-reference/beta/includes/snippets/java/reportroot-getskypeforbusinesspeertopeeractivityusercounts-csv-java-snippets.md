---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8e42ac198ddd4aaf2b19dc4c6e00fcc436f9f604
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359072"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessPeerToPeerActivityUserCountsCollectionPage getSkypeForBusinessPeerToPeerActivityUserCounts = graphClient.reports()
    .getSkypeForBusinessPeerToPeerActivityUserCounts("D7")
    .buildRequest()
    .get();

```