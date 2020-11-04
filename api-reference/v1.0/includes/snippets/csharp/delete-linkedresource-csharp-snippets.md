---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6080eec270d8698481b6cfe7a7dc539d4a5bc5b
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903447"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Todo.Lists["dfsdc-f9dfdfs-dcsda9"].Tasks["e2dc-f9cce2-dce29"].LinkedResources["f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"]
    .Request()
    .DeleteAsync();

```