---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1ba2fb25c2c7b5e6ccd12f577a366fb56bf963a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782207"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workPosition = new WorkPosition
{
    IsCurrent = true
};

await graphClient.Me.Profile.Positions["{workPosition-id}"]
    .Request()
    .UpdateAsync(workPosition);

```