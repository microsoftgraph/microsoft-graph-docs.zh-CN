---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bac6ea6efca9ef93f3a94e6055f55adabdce3c0a
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61335675"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Request()
    .GetAsync();

```