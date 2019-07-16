---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b24f66865b3df7d9b3821c0a45e7f79cb39872a5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734992"
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