---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb61fa9879536a001ae3ad5bf014f4c3807700de
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209317"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordlessMicrosoftAuthenticatorAuthenticationMethod passwordlessMicrosoftAuthenticatorAuthenticationMethod = graphClient.me().authentication().passwordlessMicrosoftAuthenticatorMethods("R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1")
    .buildRequest()
    .get();

```