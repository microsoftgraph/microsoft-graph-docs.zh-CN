---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9585993d5775d2ee2c7bd31938735580e49e34ed
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210921"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceHealthCollectionPage healthOverviews = graphClient.admin().serviceAnnouncement().healthOverviews()
    .buildRequest()
    .expand("issues")
    .get();

```