---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7e212c48b0906af44a4571cc99e6071ed8b9313d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892351"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessOrganizerActivityMinuteCounts('D7')
    .buildRequest()
    .get();

```