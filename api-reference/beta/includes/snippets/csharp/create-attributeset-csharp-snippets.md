---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e59c959a722627f7590408ea38ede08ecf6a3842
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226507"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attributeSet = new AttributeSet
{
    Id = "Engineering",
    Description = "Attributes for engineering team",
    MaxAttributesPerSet = 25
};

await graphClient.Directory.AttributeSets
    .Request()
    .AddAsync(attributeSet);

```