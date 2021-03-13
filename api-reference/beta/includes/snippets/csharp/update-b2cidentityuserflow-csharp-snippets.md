---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c1b965bdbc77f76be4a9812cf52e391edc53e66
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806465"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cIdentityUserFlow = new B2cIdentityUserFlow
{
    IsLanguageCustomizationEnabled = true,
    DefaultLanguageTag = "en"
};

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"]
    .Request()
    .UpdateAsync(b2cIdentityUserFlow);

```