---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a002b9ebed46d7bc698e02c0fb2577858f698eb7
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580672"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schema = await graphClient.Connections["{externalConnectors.externalConnection-id}"].Schema
    .Request()
    .GetAsync();

```