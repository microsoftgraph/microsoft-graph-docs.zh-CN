---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: daebe832633cac11c28102e2efc7fcfbcdc18e29
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579982"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connections = await graphClient.Connections
    .Request()
    .GetAsync();

```