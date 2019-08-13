---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 100d672ae20008834348c31d54814dbf41a988ac
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321794"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointActivityUserDetail("D7")
    .Request()
    .GetAsync();

```