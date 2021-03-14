---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7cb57bd8274e62335134993b2ffde89928dc6b7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797711"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extensionProperty = new ExtensionProperty
{
    Name = "extensionName",
    DataType = "string",
    TargetObjects = new List<String>()
    {
        "Application"
    }
};

await graphClient.Applications["{application-id}"].ExtensionProperties
    .Request()
    .AddAsync(extensionProperty);

```