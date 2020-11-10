---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d42aecd2ed10f3fae691cbff8988dd1e0a593140
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953123"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttribute identityUserFlowAttribute = new IdentityUserFlowAttribute();
identityUserFlowAttribute.description = "Your new hobby";

graphClient.identity().userFlowAttributes("extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby")
    .buildRequest()
    .patch(identityUserFlowAttribute);

```