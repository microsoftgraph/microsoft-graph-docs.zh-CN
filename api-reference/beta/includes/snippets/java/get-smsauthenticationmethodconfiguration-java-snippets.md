---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce6621f30ed8efae07d0ed2fdc870b08b09ee54d33aed277735c1ac4a330b561
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278272"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationMethodConfiguration authenticationMethodConfiguration = graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("sms")
    .buildRequest()
    .get();

```