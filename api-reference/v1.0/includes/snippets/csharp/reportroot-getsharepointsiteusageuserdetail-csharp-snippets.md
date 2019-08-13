---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 96d7501e085b729a52ae11084d93cbff9e5ce045
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321798"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointSiteUsageDetail("D7")
    .Request()
    .GetAsync();

```