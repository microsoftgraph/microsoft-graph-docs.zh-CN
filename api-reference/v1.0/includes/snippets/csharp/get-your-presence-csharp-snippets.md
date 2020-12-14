---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 172534fbb96208b3337521dfdaeaa5823bf345c0
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var presence = await graphClient.Me.Presence
    .Request()
    .GetAsync();

```