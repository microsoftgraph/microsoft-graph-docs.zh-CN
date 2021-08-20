---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0912d6c6af50540e62874191592bd7a7141c5d2664244b725845907a6e02578
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104448"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    BusinessPhones = new List<String>()
    {
        "+1 425 555 0109"
    },
    OfficeLocation = "18/2111"
};

await graphClient.Users["{user-id}"]
    .Request()
    .UpdateAsync(user);

```