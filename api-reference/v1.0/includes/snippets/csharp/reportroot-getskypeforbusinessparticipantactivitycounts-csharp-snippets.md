---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4c3ecf1079f0f35b8d4ef65be0f13009c6053b2c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885262"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessParticipantActivityCounts('D7')
    .Request()
    .GetAsync();

```