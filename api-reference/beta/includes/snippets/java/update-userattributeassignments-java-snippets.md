---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83539e2126a3cf7ee0ebc0b31cbe9843d478b30ad0cce08a4cd934eef18d4fba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162391"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignment identityUserFlowAttributeAssignment = new IdentityUserFlowAttributeAssignment();
identityUserFlowAttributeAssignment.userInputType = IdentityUserFlowAttributeInputType.TEXT_BOX;

graphClient.identity().b2cUserFlows("{b2cIdentityUserFlowId}").userAttributeAssignments("{id}")
    .buildRequest()
    .patch(identityUserFlowAttributeAssignment);

```