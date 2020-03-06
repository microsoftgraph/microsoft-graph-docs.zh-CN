---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d143ded08275c82b9a00e1370a3e7258e7a64242
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997114"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Application application = new Application();
application.displayName = "Display name";

graphClient.applications()
    .buildRequest()
    .post(application);

```