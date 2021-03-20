---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06abb120eb55090cb76ec8fdfc2471ca197f4bbc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944445"
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

graphClient.identity().b2xUserFlows("B2X_1_Partner").userAttributeAssignments()
    .buildRequest()
    .post(identityUserFlowAttributeAssignment);

```