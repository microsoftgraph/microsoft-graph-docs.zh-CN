---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9e438144ffbc6aef8ea04392c0cc527bc9263c3a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893426"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointSiteUsageFileCounts('D7')
    .buildRequest()
    .get();

```