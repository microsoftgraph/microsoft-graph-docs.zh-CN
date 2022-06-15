---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 895e809ec9e6ac5c5d3c3893bed797d1da437027
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094505"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationMethodConfiguration authenticationMethodConfiguration = new AuthenticationMethodConfiguration();
authenticationMethodConfiguration.isUsableOnce = true;

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("temporaryAccessPass")
    .buildRequest()
    .patch(authenticationMethodConfiguration);

```