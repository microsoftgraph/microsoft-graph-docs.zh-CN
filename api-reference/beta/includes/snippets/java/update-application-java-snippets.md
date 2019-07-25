---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6fdd4bb3941b197b02b63a2f7558d82f6b2de17e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856791"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Application application = new Application();
application.allowPublicClient = false;
application.displayName = "New display name";

graphClient.applications("{id}")
    .buildRequest()
    .patch(application);

```