---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fcf2486f9d321791874b9a449d35056f7345256c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508431"
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