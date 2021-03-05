---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3b758dd4f486b230d6483f505a3ba3baa73bb5f
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470557"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentDefaults = await graphClient.Education.Classes["{id}"].AssignmentDefaults
    .Request()
    .GetAsync();

```