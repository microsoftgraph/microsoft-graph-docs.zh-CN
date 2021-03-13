---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 794f8e1e12414a561183b649c423e213b90f1d43
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781057"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Connections["{externalConnection-id}"]
    .Request()
    .DeleteAsync();

```