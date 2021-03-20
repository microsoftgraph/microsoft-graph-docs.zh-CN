---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a9d1e477ef83a446048c6d6dcb44221aef2d700
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942151"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TiIndicator tiIndicator = new TiIndicator();
tiIndicator.description = "description-updated";

graphClient.security().tiIndicators("{id}")
    .buildRequest()
    .patch(tiIndicator);

```