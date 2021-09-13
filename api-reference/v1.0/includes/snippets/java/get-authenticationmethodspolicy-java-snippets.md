---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 225c6663a73282cd0c166cf3c76ccd212e52813fa994cfb353645974b2f9ec93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105017"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationMethodsPolicy authenticationMethodsPolicy = graphClient.policies().authenticationMethodsPolicy()
    .buildRequest()
    .get();

```