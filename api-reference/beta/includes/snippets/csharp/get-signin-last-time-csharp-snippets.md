---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 639869647f7c5e185bc9590de884bae53e12d5a8f487ac3641f9ef4051fb9240
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378553"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Select("displayName,userPrincipalName,signInActivity")
    .GetAsync();

```