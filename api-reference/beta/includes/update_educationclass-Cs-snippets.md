---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 500cb0fac3a06d64fbf64c68d9bff132d6a0a022
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461311"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = new EducationClass
{
    Description = "History - World History 1",
    DisplayName = "World History Level 1"
};

await graphClient.Education.Classes["11014"]
    .Request()
    .UpdateAsync(educationClass);

```