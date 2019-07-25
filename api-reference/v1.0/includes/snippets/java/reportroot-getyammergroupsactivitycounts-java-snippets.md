---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c35621c97eb281d806344fa0dbbea94a85915b6c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881238"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerGroupsActivityCounts('D7')
    .buildRequest()
    .get();

```