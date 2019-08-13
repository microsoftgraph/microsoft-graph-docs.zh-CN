---
description: 自动生成的文件。 不修改
ms.openlocfilehash: edcea75e42823f58547c8effc68af407f52b6195
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349259"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessActivityUserCounts("D7")
    .Request()
    .GetAsync();

```