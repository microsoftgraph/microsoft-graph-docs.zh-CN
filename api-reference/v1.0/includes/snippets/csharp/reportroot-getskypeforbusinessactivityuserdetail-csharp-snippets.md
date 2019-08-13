---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e396bc1570de5232516dbdd3c399ed75e59c562f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349205"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessActivityUserDetail("D7")
    .Request()
    .GetAsync();

```