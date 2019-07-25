---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bba30ad8658616231688dc101a9a694d3297f26d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873554"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365ActivationsUserCountsCollectionPage getOffice365ActivationsUserCounts = graphClient.reports()
    .getOffice365ActivationsUserCounts()
    .buildRequest()
    .get();

```