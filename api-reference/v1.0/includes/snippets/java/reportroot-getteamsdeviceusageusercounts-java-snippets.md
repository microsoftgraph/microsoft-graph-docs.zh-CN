---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1c38c012271c8692c830f63aa8ea02f29bde12c7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855614"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getTeamsDeviceUsageUserCounts('D7')
    .buildRequest()
    .get();

```