---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70a740c36c74229efdf854d8d3fc6948df0fa1ac
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683814"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = new OpenTypeExtension
{
    ExtensionName = "Com.Contoso.Deal",
    AdditionalData = new Dictionary<string, object>()
    {
        {"companyName", "Alpine Skis"},
        {"dealValue", "1010100"},
        {"expirationDate", "2015-07-03T13:04:00Z"}
    }
};

await graphClient.Groups["f5480dfd-7d77-4d0b-ba2e-3391953cc74a"].Events["AAMkADVl17IsAAA="].Extensions
    .Request()
    .AddAsync(extension);

```