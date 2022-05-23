---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a31f40e1da6eebc749de588bdddd5f4a0371fc2
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629449"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Education.Classes["{educationClass-id}"].Assignments
    .Delta()
    .Request()
    .GetAsync();

```