---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 43d77ed5994484661fe90e5a0eebb1feaea5eda5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872305"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessOrganizerActivityCountsCollectionPage getSkypeForBusinessOrganizerActivityCounts = graphClient.reports()
    .getSkypeForBusinessOrganizerActivityCounts('D7')
    .buildRequest()
    .get();

```