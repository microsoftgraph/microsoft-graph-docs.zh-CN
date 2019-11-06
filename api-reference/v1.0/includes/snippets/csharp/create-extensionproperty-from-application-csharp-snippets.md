---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e5fb1b431dbc94a63bd330fdd1d1ac4d12b966d
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998970"
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

await graphClient.Applications["{id}"].ExtensionProperties
    .Request()
    .AddAsync(extensionProperty);

```