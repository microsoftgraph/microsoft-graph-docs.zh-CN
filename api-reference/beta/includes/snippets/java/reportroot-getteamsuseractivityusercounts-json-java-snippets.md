---
description: 自动生成的文件。 不修改
ms.openlocfilehash: de62dac41bc577d4c2411c4cb30149cf040d2add
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871687"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsUserActivityUserCountsCollectionPage getTeamsUserActivityUserCounts = graphClient.reports()
    .getTeamsUserActivityUserCounts('D7')
    .buildRequest()
    .get();

```