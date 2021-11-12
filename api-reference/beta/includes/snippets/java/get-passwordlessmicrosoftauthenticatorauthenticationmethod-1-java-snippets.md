---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 942aeed75c52315d82676c72b472bdd8b9a04e647a6caccaa01c0340c3d365d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220802"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordlessMicrosoftAuthenticatorAuthenticationMethod passwordlessMicrosoftAuthenticatorAuthenticationMethod = graphClient.me().authentication().passwordlessMicrosoftAuthenticatorMethods("R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1")
    .buildRequest()
    .get();

```