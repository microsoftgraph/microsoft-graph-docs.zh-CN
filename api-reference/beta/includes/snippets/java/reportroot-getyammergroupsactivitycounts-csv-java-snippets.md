---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9e0f5423284f48981303b4b0e22df515c04a48f6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358457"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerGroupsActivityCountsCollectionPage getYammerGroupsActivityCounts = graphClient.reports()
    .getYammerGroupsActivityCounts("D7")
    .buildRequest()
    .get();

```