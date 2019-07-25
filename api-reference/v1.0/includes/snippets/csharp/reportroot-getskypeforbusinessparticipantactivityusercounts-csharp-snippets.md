---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 77e68d95ffb876395d4e90bb156688aac4ea7767
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892283"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessParticipantActivityUserCounts('D7')
    .Request()
    .GetAsync();

```