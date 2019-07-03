---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b81c390c250d4f1105535bdb7eb407bd70a1d030
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520470"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.DirectoryObjects["{id}"]
    .Request()
    .GetAsync();

```