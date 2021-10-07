---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a958adec7fb97fb23d1477ac58d17af53ac0728817688a5fe2094aed6fdb4634
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220797"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("passwordlessMicrosoftAuthenticator")
    .buildRequest()
    .delete();

```