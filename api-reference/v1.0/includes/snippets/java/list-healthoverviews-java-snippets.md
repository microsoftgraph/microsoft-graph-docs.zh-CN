---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71382c1ac0d89af97e353035890c4dfb6d448134
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259130"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceHealthCollectionPage healthOverviews = graphClient.admin().serviceAnnouncement().healthOverviews()
    .buildRequest()
    .get();

```