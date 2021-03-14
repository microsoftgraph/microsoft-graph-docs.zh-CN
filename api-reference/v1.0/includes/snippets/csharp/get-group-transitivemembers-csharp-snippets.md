---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 911c2d5ec623e1f6c4c45b95fc9afac557a84b0b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783007"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMembers = await graphClient.Groups["{group-id}"].TransitiveMembers
    .Request()
    .GetAsync();

```