---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8db43bb419ccbea747bdadf1b3d2cb7affcccde8
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347935"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teamwork.Devices["{teamworkDevice-id}"]
    .Restart()
    .Request()
    .PostAsync();

```