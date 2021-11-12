---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7c29056cc27acdbb4f60ea92a019f91cc64f35693652a5495590f2052d7cd7a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279582"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPhone = new ItemPhone
{
    DisplayName = "Car Phone",
    Number = "+7 499 342 22 13"
};

await graphClient.Me.Profile.Phones
    .Request()
    .AddAsync(itemPhone);

```