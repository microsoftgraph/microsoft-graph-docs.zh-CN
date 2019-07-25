---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3c2b0a191feb12a103688ca83067209a182c62af
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872139"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessOrganizerActivityUserCountsCollectionPage getSkypeForBusinessOrganizerActivityUserCounts = graphClient.reports()
    .getSkypeForBusinessOrganizerActivityUserCounts('D7')
    .buildRequest()
    .get();

```