---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 244d55c40a98f7b4bf70961e458ff293417ef16a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871120"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskDetection riskDetection = graphClient.riskDetections("c2b6c2b9-dddc-acd0-2b39-d519d803dbc3")
    .buildRequest()
    .get();

```