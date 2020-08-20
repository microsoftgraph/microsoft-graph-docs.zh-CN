---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd062c6dbe22569673f048b903b77f03773fc1c9
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821158"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personName = new PersonName
{
    Nickname = "Kesha"
};

await graphClient.Me.Profile.Names["{id}"]
    .Request()
    .UpdateAsync(personName);

```