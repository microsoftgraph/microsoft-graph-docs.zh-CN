---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b226f87522412109ff3163236b5a0554adb40105
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493344"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = await graphClient.Education.Schools["{school-id}"]
    .Request()
    .GetAsync();

```