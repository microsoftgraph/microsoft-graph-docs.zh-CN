---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bb9e14f18ceacb2a2494b25ee5ed4f8aac04981
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779800"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personName = new PersonName
{
    Nickname = "Kesha"
};

await graphClient.Me.Profile.Names["{personName-id}"]
    .Request()
    .UpdateAsync(personName);

```