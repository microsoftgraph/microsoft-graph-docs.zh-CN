---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0e497b72e6ea2627b4842c8f33fb8884ae652fcc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34464028"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessParticipantActivityMinuteCounts = await graphClient.Reports.GetSkypeForBusinessParticipantActivityMinuteCounts('D7')
    .Request()
    .GetAsync();

```