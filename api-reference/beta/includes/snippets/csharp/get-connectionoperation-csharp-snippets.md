---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 587f401e896f58212f98024f21384ab6d1629bf7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798685"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectionOperation = await graphClient.Connections["{externalConnection-id}"].Operations["{connectionOperation-id}"]
    .Request()
    .GetAsync();

```