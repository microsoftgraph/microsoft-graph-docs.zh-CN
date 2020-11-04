---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06cb64fef9e73d34c66c00cafbffdc85b64840c2
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903877"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlowAttribute = new IdentityUserFlowAttribute
{
    DisplayName = "Hobby",
    Description = "Your hobby",
    DataType = IdentityUserFlowAttributeDataType.String
};

await graphClient.Identity.UserFlowAttributes
    .Request()
    .AddAsync(identityUserFlowAttribute);

```