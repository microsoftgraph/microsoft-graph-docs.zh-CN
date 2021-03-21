---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca2241e5bc3dbe5a77d07d7ca769d1c8be7ded76
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976658"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentitySecurityDefaultsEnforcementPolicy identitySecurityDefaultsEnforcementPolicy = new IdentitySecurityDefaultsEnforcementPolicy();
identitySecurityDefaultsEnforcementPolicy.isEnabled = false;

graphClient.policies().identitySecurityDefaultsEnforcementPolicy()
    .buildRequest()
    .patch(identitySecurityDefaultsEnforcementPolicy);

```