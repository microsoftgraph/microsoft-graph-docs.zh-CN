---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d13dfb12675ab394d92fc2a8edf005ed4535afe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806185"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Schedule.Shifts["{shift-id}"]
    .Request()
    .DeleteAsync();

```