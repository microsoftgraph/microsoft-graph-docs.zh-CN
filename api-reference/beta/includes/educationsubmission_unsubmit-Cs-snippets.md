---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 19a31bd49fcc9dc96a215f6e0c45a6a0f533786f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436927"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11021"].Assignments["19002"].Submissions["850f51b7"]
    .Unsubmit()
    .Request()
    .PostAsync();

```