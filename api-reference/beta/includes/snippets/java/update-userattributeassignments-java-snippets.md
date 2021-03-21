---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c906e25ca81a5a7e5f2c0598fbdd047fb5b6687
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980846"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignment identityUserFlowAttributeAssignment = new IdentityUserFlowAttributeAssignment();
identityUserFlowAttributeAssignment.userInputType = IdentityUserFlowAttributeInputType.TEXT_BOX;

graphClient.identity().b2cUserFlows("{b2cIdentityUserFlowId}").userAttributeAssignments("{id}")
    .buildRequest()
    .patch(identityUserFlowAttributeAssignment);

```