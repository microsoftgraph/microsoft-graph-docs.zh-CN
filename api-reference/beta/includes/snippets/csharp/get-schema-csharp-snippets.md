---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b12852fef1aeac108e4bcebc6d706aabd0cb2cb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808454"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schema = await graphClient.External.Connections["{externalConnection-id}"].Schema
    .Request()
    .GetAsync();

```