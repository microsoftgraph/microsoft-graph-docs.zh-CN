---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a31f40e1da6eebc749de588bdddd5f4a0371fc2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137712"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Education.Classes["{educationClass-id}"].Assignments
    .Delta()
    .Request()
    .GetAsync();

```