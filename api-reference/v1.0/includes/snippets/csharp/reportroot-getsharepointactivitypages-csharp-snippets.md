---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 266c2447f5d1b2e24fa267c8687d430638f6eca0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492971"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSharePointActivityPages('D7')
    .Request()
    .GetAsync();

```