---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b24f66865b3df7d9b3821c0a45e7f79cb39872a5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475554"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = new EducationClass
{
    Description = "History - World History 1",
    DisplayName = "World History Level 1"
};

await graphClient.Education.Classes["{class-id}"]
    .Request()
    .UpdateAsync(educationClass);

```