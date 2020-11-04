---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57ffcd9ce77888fbba7cb4314fa2fe1bbceb539e
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903979"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlowAttribute = new IdentityUserFlowAttribute
{
    Description = "Your new hobby"
};

await graphClient.Identity.UserFlowAttributes["extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby"]
    .Request()
    .UpdateAsync(identityUserFlowAttribute);

```