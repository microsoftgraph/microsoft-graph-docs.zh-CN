---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e90b25b3c914d0bbc722b0556021e558fa067fefa624e5f62e28133d57f4ac33
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332760"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Self help community for library",
    DisplayName = "Library Assist",
    GroupTypes = new List<String>()
    {
        "Unified"
    },
    MailEnabled = true,
    MailNickname = "library",
    SecurityEnabled = false
};

await graphClient.Groups
    .Request()
    .AddAsync(group);

```