---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 54fc34ec937d872a4328eba95e987f744c278edd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453248"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{teamId}"].Schedule.Shifts["{shiftId}"]
    .Request()
    .DeleteAsync();

```