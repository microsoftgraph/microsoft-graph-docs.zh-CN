---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 100e28b47682812022e84bd1f4aca665956c1df0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871721"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsUserActivityCountsCollectionPage getTeamsUserActivityCounts = graphClient.reports()
    .getTeamsUserActivityCounts('D7')
    .buildRequest()
    .get();

```