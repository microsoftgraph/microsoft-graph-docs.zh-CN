---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ccb82d3d8bf911a63dbf7b09e5847ce1a103fd80
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48984248"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{id}"].Manager.Reference
    .Request()
    .PutAsync("{id}");

```