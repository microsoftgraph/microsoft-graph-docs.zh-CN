---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b8ee54595523d2618e2dd93a72282cb4e59f23eb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871949"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessParticipantActivityUserCounts = await graphClient.Reports
    .GetSkypeForBusinessParticipantActivityUserCounts('D7')
    .Request()
    .GetAsync();

```