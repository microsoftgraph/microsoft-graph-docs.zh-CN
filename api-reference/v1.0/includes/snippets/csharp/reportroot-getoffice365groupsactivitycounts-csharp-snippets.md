---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 82dfa20c78e5e4be7ee7c0ba9b08090d51520800
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467796"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOffice365GroupsActivityCounts('D7')
    .Request()
    .GetAsync();

```