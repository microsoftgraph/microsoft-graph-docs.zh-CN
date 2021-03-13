---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 306439cdff4d0aff87942a575facbdaf7e2442f6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807012"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workPosition = await graphClient.Me.Profile.Positions["{workPosition-id}"]
    .Request()
    .GetAsync();

```