---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06cb64fef9e73d34c66c00cafbffdc85b64840c2
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920845"
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