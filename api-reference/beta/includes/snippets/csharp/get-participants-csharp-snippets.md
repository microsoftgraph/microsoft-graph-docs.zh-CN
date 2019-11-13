---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dec143c983c392f7cbe7a80ea6384d3752c7ffa
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302396"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participants = await graphClient.Communications.Calls["7531d31f-d10d-44de-802f-c569dbca451c"].Participants
    .Request()
    .GetAsync();

```