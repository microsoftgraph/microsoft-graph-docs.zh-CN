---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22aa8f05136e84aff4b7f0206d068d536bc749bf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797235"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = new EducationClass
{
    Description = "History - World History 1",
    DisplayName = "World History Level 1"
};

await graphClient.Education.Classes["{educationClass-id}"]
    .Request()
    .UpdateAsync(educationClass);

```