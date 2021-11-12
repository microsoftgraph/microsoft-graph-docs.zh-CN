---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0af5b3c9146cfda858ac57fb9592e22c9f76ed49f3a4438b6ef1fa2cb4e7fd5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163942"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemEmail = new ItemEmail
{
    Address = "Innocenty.Popov@adventureworks.com"
};

await graphClient.Me.Profile.Emails
    .Request()
    .AddAsync(itemEmail);

```