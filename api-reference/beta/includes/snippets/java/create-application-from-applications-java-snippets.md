---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d143ded08275c82b9a00e1370a3e7258e7a64242
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962002"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Application application = new Application();
application.displayName = "Display name";

graphClient.applications()
    .buildRequest()
    .post(application);

```