---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9e95ebb0068827b80c36d193c2e770de159f53a6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722689"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"]
    .Renew()
    .Request()
    .PostAsync();

```