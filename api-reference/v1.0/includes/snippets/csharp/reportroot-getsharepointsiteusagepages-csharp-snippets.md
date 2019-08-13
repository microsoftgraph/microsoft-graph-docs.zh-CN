---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e61ac2689d5e9f50aef4a4d8abd0c3450a9cfe18
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357993"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointSiteUsagePages("D7")
    .Request()
    .GetAsync();

```