---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 259d227796b61ab284415945d522697d5ddc4735
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794180"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var webAccount = new WebAccount
{
    WebUrl = "https://github.com/innocenty.popov"
};

await graphClient.Me.Profile.WebAccounts["{webAccount-id}"]
    .Request()
    .UpdateAsync(webAccount);

```