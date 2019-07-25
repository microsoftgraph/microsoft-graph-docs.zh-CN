---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 08df1a545a9cd144fa4f2df700d36ecae23c2401
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712044"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var endpoints = await graphClient.Groups["{id}"].Endpoints
    .Request()
    .GetAsync();

```