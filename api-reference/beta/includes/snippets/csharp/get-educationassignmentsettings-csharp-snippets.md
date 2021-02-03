---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 693e94a6959a79910b1146103151dcb77a3b73b8
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092532"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentSettings = await graphClient.Education.Classes["{id}"].AssignmentSettings
    .Request()
    .GetAsync();

```