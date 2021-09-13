---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84050a890146646df975eabb7d900fb3f9a6174fe23b02de43b56bafc855bed1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215912"
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