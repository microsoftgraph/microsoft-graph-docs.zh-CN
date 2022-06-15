---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cb36cb7bccd997a02e2d517149c25bb4b1fcbbc
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093203"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationMethodConfiguration authenticationMethodConfiguration = graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("temporaryAccessPass")
    .buildRequest()
    .get();

```