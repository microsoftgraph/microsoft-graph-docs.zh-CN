---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7408d583283237d3f6e677db84220df0d846ef6b
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52254204"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRubric = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Rubric
    .Request()
    .GetAsync();

```