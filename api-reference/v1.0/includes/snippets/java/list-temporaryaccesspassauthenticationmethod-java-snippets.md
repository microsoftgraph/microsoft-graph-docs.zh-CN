---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7ba1cc612fa1c0ab46f2e775168271a8b9aa48a
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093406"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TemporaryAccessPassAuthenticationMethodCollectionPage temporaryAccessPassMethods = graphClient.users("071cc716-8147-4397-a5ba-b2105951cc0b").authentication().temporaryAccessPassMethods()
    .buildRequest()
    .get();

```