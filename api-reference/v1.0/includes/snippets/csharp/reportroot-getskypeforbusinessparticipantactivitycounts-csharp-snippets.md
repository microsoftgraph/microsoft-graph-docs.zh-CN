---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6be8ed8ff6b71bf2f96fab410541db86e01ca2f2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320708"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessParticipantActivityCounts("D7")
    .Request()
    .GetAsync();

```