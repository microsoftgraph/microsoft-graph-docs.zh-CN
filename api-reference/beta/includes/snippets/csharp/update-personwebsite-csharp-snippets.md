---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f726253567706243fed51bc32045adb238443b7b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780869"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personWebsite = new PersonWebsite
{
    Description = "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway"
};

await graphClient.Me.Profile.Websites["{personWebsite-id}"]
    .Request()
    .UpdateAsync(personWebsite);

```