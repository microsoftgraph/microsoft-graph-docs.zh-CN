---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 81ea9a8ca7ce30f89efed2606dee77afe152ebb6
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933819"
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
        "550fae72-d251-43ec-868c-373732c2704f",
        "72f988bf-86f1-41af-91ab-2d7cd011db47"
    }
};

await graphClient.App.Calls["{id}"].AudioRoutingGroups["{id}"]
    .Request()
    .UpdateAsync(audioRoutingGroup);

```