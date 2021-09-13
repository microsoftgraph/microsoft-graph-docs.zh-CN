---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e2faa9d24c500b0138cce18a031875c97b9641cedbaa600b76d3ec102a2dc78
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162579"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Library Assist",
    DisplayName = "Library Assist",
    GroupTypes = new List<String>()
    {
        "Unified"
    },
    MailEnabled = true,
    MailNickname = "library-help"
};

await graphClient.Groups["{group-id}"]
    .Request()
    .UpdateAsync(group);

```