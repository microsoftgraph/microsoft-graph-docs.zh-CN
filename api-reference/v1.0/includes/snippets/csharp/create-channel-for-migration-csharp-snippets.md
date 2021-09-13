---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26ee3ab9fcfd6e6e54eb271c250f73d9ab5939630cea8b229995e679974977f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279691"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    DisplayName = "Import_150958_99z",
    Description = "Import_150958_99z",
    CreatedDateTime = DateTimeOffset.Parse("2020-03-14T11:22:17.067Z"),
    AdditionalData = new Dictionary<string, object>()
    {
        {"@microsoft.graph.channelCreationMode", "migration"}
    }
};

await graphClient.Teams["{team-id}"].Channels
    .Request()
    .AddAsync(channel);

```