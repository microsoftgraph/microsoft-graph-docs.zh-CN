---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ac438bd8d0dd9470eff80efaacd7b346a3baa5c8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321734"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointActivityPages("D7")
    .Request()
    .GetAsync();

```