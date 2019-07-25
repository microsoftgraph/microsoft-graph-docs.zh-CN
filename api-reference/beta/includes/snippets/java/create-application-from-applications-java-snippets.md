---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 538bce8a2709065a0b4a2de9bb0e5af83d62692b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855202"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Application application = new Application();
application.allowPublicClient = true;
application.displayName = "Display name";

graphClient.applications()
    .buildRequest()
    .post(application);

```