---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd7e66968d6165ad44a7e107d924db74d253ee0c
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302550"
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

await graphClient.Communications.Calls["{id}"].AudioRoutingGroups
    .Request()
    .AddAsync(audioRoutingGroup);

```