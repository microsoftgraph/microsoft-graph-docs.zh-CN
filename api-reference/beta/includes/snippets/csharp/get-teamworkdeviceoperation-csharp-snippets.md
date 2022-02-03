---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4afc7300662dadd97b4dabc8e76039dbf335fb42
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348297"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkDeviceOperation = await graphClient.Teamwork.Devices["{teamworkDevice-id}"].Operations["{teamworkDeviceOperation-id}"]
    .Request()
    .GetAsync();

```