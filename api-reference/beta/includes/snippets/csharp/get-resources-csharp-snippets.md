---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c370d7de87aa55b21de36ab4449e3020fc9491a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470462"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var resources = await graphClient.Education.Classes["11012"].Assignments["19002"].Resources
    .Request()
    .GetAsync();

```