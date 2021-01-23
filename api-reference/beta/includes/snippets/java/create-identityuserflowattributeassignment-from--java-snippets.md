---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b57a157534283b4ad0107b03d9caaad30533fffa
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944717"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignment identityUserFlowAttributeAssignment = new IdentityUserFlowAttributeAssignment();
identityUserFlowAttributeAssignment.isOptional = false;
identityUserFlowAttributeAssignment.requiresVerification = false;
identityUserFlowAttributeAssignment.userInputType = IdentityUserFlowAttributeInputType.TEXT_BOX;
identityUserFlowAttributeAssignment.displayName = "Shoe size";
LinkedList<UserAttributeValuesItem> userAttributeValuesList = new LinkedList<UserAttributeValuesItem>();
identityUserFlowAttributeAssignment.userAttributeValues = userAttributeValuesList;
IdentityUserFlowAttribute userAttribute = new IdentityUserFlowAttribute();
userAttribute.id = "extension_guid_shoeSize";
identityUserFlowAttributeAssignment.userAttribute = userAttribute;

graphClient.identity().b2cUserFlows("B2C_1_Consumer").userAttributeAssignments()
    .buildRequest()
    .post(identityUserFlowAttributeAssignment);

```