---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b0da7cf0784ada5a72967d586216045f938119888d031f7042a193720c7734c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164162"
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