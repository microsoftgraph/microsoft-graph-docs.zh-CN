---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2459846b0ac543f0bc4164ff4206b1d941d597ba647faf453b502d58495ac585
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106025"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentitySecurityDefaultsEnforcementPolicy identitySecurityDefaultsEnforcementPolicy = graphClient.policies().identitySecurityDefaultsEnforcementPolicy()
    .buildRequest()
    .get();

```