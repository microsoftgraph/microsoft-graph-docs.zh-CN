---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b76d66dba1a6598eb4d450baccdf7eab829c0c13
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411841"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extensionProperty = new ExtensionProperty
{
    Name = "jobGroup",
    DataType = "String",
    TargetObjects = new List<String>()
    {
        "User"
    }
};

await graphClient.Applications["{application-id}"].ExtensionProperties
    .Request()
    .AddAsync(extensionProperty);

```