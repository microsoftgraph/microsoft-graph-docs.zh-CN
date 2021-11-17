---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bded4c3fe8a53f1876fba1ce33a6f60a660efe3675434b572b131b327eb7dab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162164"
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