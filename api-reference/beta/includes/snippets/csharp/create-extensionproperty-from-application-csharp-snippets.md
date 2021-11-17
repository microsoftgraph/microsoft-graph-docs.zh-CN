---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6fd8ce0454dad28059197902eba2ddb0bc140b7f7f26c094a2f48edb6b51c08
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161311"
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