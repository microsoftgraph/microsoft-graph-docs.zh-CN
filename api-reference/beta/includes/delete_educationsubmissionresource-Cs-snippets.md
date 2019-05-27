---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 589b89682784a3ea867fe5e018b25c97ce1fefa8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438383"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11021"].Assignments["19002"].Submissions["850f51b7"].Resources["f2387c3b-ec39-4bf2-a399-d7242677f024"]
    .Request()
    .DeleteAsync();

```