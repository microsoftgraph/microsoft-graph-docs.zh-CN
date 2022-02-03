---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fd681a48fd5bed3859d9d8d0b9c031a2810ea8b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347424"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkDeviceActivity = await graphClient.Teamwork.Devices["{teamworkDevice-id}"].Activity
    .Request()
    .GetAsync();

```