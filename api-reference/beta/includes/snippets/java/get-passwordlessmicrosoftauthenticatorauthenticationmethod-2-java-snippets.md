---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 918d92298cf5ceaa5b01bda29b96e2da4a101fe3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962972"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPasswordlessMicrosoftAuthenticatorAuthenticationMethodCollectionPage passwordlessMicrosoftAuthenticatorMethods = graphClient.me().authentication().passwordlessMicrosoftAuthenticatorMethods()
    .buildRequest()
    .get();

```