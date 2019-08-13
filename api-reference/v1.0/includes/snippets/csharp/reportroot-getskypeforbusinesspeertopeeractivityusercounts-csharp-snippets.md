---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 91a3cc3fd11af8ff25edea82a28491227f87bfda
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320560"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessPeerToPeerActivityUserCounts("D7")
    .Request()
    .GetAsync();

```