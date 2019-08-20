---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0c86afa73ec932cb04df80379efb8ee369f7af48
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36464994"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{item-id}"]
    .Unfollow()
    .Request()
    .DeleteAsync();

```