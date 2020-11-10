---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d3f3c4a4a9a948a9b8513111a38dfa8fef78602
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953332"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentitySecurityDefaultsEnforcementPolicy identitySecurityDefaultsEnforcementPolicy = new IdentitySecurityDefaultsEnforcementPolicy();
identitySecurityDefaultsEnforcementPolicy.isEnabled = false;

graphClient.policies().identitySecurityDefaultsEnforcementPolicy()
    .buildRequest()
    .patch(identitySecurityDefaultsEnforcementPolicy);

```