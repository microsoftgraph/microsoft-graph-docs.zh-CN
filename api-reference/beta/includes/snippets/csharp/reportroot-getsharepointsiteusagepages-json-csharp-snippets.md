---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 052a431df1b9960bce5288263c1b7595782ea854
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359734"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointSiteUsagePages = await graphClient.Reports
    .GetSharePointSiteUsagePages("D7")
    .Request()
    .GetAsync();

```