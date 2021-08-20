---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79f9a814e6841d1f86a32a25dee2dc1bd82b4e7999848fb1de17f3383b4b3431
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104449"
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

await graphClient.Me
    .Request()
    .UpdateAsync(user);

```