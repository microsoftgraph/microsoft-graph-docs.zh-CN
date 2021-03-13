---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e04bc4729049ba98cbff5702b20fc3df628bec54
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788020"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlowAttributeAssignment = new IdentityUserFlowAttributeAssignment
{
    IsOptional = false,
    RequiresVerification = false,
    UserInputType = IdentityUserFlowAttributeInputType.TextBox,
    DisplayName = "Shoe size",
    UserAttributeValues = new List<UserAttributeValuesItem>()
    {
    },
    UserAttribute = new IdentityUserFlowAttribute
    {
        Id = "extension_guid_shoeSize"
    }
};

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].UserAttributeAssignments
    .Request()
    .AddAsync(identityUserFlowAttributeAssignment);

```