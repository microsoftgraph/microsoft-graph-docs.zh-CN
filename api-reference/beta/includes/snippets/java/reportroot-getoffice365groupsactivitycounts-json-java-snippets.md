---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 70b3b15952cc2191bee96ec8066706e2ca546e88
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873409"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365GroupsActivityCountsCollectionPage getOffice365GroupsActivityCounts = graphClient.reports()
    .getOffice365GroupsActivityCounts('D7')
    .buildRequest()
    .get();

```