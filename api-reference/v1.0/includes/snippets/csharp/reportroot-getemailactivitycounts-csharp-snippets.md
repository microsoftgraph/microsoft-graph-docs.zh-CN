---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 259352a2109feb3d218f51e80069a8d6c3f65998
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327451"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetEmailActivityCounts("D7")
    .Request()
    .GetAsync();

```