---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efba46894f87ac1b288faf7332997882ffd4504fd4c70a2d6d543b5229978fdb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274025"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var audioRoutingGroup = new AudioRoutingGroup
{
    Id = "oneToOne",
    RoutingMode = RoutingMode.OneToOne,
    Sources = new List<String>()
    {
        "632899f8-2ea1-4604-8413-27bd2892079f"
    },
    Receivers = new List<String>()
    {
        "550fae72-d251-43ec-868c-373732c2704f"
    }
};

await graphClient.Communications.Calls["{call-id}"].AudioRoutingGroups
    .Request()
    .AddAsync(audioRoutingGroup);

```