---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 126fb4ecc62b18450f6e6c5408b4eb4d4b76f061
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348380"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var softwareType = TeamworkSoftwareType.TeamsClient;

var softwareVersion = "1.0.96.22";

await graphClient.Teamwork.Devices["{teamworkDevice-id}"]
    .UpdateSoftware(softwareType,softwareVersion)
    .Request()
    .PostAsync();

```