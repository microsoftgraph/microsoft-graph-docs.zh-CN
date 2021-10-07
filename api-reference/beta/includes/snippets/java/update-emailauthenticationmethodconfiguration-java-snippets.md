---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ab97ee41985782537ed211427525ae844c21f7c5bd13948109e75596225e5be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219961"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EmailAuthenticationMethodConfiguration authenticationMethodConfiguration = new EmailAuthenticationMethodConfiguration();
authenticationMethodConfiguration.allowExternalIdToUseEmailOtp = ExternalEmailOtpState.DISABLED;

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("email")
    .buildRequest()
    .patch(authenticationMethodConfiguration);

```