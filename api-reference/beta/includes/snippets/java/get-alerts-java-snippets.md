---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1889a652eb8c6029041095b818be4b9925decd45
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855402"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAlertCollectionPage alerts = graphClient.security().alerts()
    .buildRequest()
    .get();

```