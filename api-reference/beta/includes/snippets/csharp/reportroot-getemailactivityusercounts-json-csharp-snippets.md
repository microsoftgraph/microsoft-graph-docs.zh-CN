---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 57dd07828336a98cbf965d809296630f6a1cd47c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874031"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailActivityUserCounts = await graphClient.Reports
    .GetEmailActivityUserCounts('D7')
    .Request()
    .GetAsync();

```