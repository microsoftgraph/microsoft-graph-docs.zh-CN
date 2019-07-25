---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ab1f76cf4d45e2eb9059d90e00e1f8bd869e1c95
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885263"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessParticipantActivityCounts('D7')
    .buildRequest()
    .get();

```