---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2341ea99a64c67c3ef5f6f45c2d1a20b3e966f94
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689211"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignment identityUserFlowAttributeAssignment = new IdentityUserFlowAttributeAssignment();
identityUserFlowAttributeAssignment.userInputType = IdentityUserFlowAttributeInputType.TEXT_BOX;

graphClient.identity().b2cUserFlows("{b2cIdentityUserFlowId}").userAttributeAssignments("{id}")
    .buildRequest()
    .patch(identityUserFlowAttributeAssignment);

```