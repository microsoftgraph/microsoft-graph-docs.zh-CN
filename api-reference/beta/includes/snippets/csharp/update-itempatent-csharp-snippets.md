---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1c99820b14af83766a78283331273d8f2359416ec0d575cb19c1dcb3286ce19
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220884"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPatent = new ItemPatent
{
    Number = "USPTO-3954432633",
    WebUrl = "https://patents.gov/3954432633"
};

await graphClient.Users["{user-id}"].Profile.Patents["{itemPatent-id}"]
    .Request()
    .UpdateAsync(itemPatent);

```