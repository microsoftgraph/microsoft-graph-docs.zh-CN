---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 556de9e35d2fc2d3d1d7d8d2ea9be1f7a11962bb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967452"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Application application = new Application();
application.displayName = "Display name";

graphClient.applications()
    .buildRequest()
    .post(application);

```