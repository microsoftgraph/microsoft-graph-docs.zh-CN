---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89c9c1060dcfc994aaf0bdd59a17dffb803fbdf1
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60560575"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentResource = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Resources["{educationAssignmentResource-id}"]
    .Request()
    .GetAsync();

```