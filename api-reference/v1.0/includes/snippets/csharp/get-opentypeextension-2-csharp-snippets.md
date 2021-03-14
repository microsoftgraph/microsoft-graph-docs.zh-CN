---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6299d641b02960563a0a06b11817a7caf64ec367
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790455"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = await graphClient.Groups["{group-id}"].Events["{event-id}"].Extensions["{extension-id}"]
    .Request()
    .GetAsync();

```