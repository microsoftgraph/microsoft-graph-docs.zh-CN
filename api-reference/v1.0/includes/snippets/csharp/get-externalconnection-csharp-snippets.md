---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0aedf0d88214b5fa1f69ff85826990c718bf8ca0
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580022"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalConnection = await graphClient.Connections["{externalConnectors.externalConnection-id}"]
    .Request()
    .GetAsync();

```