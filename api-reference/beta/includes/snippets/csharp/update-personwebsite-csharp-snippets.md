---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1baf58a78435e905436656d234ee06bea5ab696a
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819827"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personWebsite = new PersonWebsite
{
    Description = "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway"
};

await graphClient.Me.Profile.Websites["{id}"]
    .Request()
    .UpdateAsync(personWebsite);

```