---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 500cb0fac3a06d64fbf64c68d9bff132d6a0a022
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604586"
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