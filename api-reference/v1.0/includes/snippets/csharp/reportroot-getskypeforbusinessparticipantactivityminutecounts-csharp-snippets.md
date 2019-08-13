---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f9d9a2b4c76fdcb2186000da275c2eab35b04d77
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320654"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessParticipantActivityMinuteCounts("D7")
    .Request()
    .GetAsync();

```