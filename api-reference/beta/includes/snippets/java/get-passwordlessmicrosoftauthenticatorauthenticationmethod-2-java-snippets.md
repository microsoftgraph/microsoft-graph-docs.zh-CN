---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76e4c1b201ad153b0a65b4b013c2b688734b142bb58a53778da758a2d662d7a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278380"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordlessMicrosoftAuthenticatorAuthenticationMethodCollectionPage passwordlessMicrosoftAuthenticatorMethods = graphClient.me().authentication().passwordlessMicrosoftAuthenticatorMethods()
    .buildRequest()
    .get();

```