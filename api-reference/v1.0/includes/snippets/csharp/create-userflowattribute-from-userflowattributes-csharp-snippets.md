---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8d1d1607f4fe23195c596bf92ae97289b5d2005b6c876ba27e91ee647a9e12d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163269"
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