---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d95624bf84032a06e1610c1a159572650ff1432505349394f1e19360e1ca09d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332448"
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

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].UserAttributeAssignments
    .Request()
    .AddAsync(identityUserFlowAttributeAssignment);

```