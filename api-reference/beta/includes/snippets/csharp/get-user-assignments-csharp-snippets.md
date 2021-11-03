---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa8bc94e1c9e999ed1581507d9a80b94f522e079
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730184"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.Education.Users["{educationUser-id}"].Assignments
    .Request()
    .GetAsync();

```