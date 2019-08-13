---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3124d05ec92662f5191b411b3165ed77d12f1842
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308341"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityCounts = await graphClient.Reports
    .GetOffice365GroupsActivityCounts("D7")
    .Request()
    .GetAsync();

```