---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 477ad9a4749da9432ef27d34c7666996e251ab99
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978645"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TiIndicatorCollectionPage tiIndicators = graphClient.security().tiIndicators()
    .buildRequest()
    .get();

```