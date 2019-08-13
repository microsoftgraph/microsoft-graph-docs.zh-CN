---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fa861a45d2ce750e6fbe194ed60c70c67f0ec12f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321731"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointActivityFileCounts("D7")
    .Request()
    .GetAsync();

```