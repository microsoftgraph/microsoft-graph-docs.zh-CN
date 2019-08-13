---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1842dcaf275c1adffc2e6c0704dd12bfcbb9ba9a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359902"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointActivityUserDetail = await graphClient.Reports
    .GetSharePointActivityUserDetail("D7")
    .Request()
    .GetAsync();

```