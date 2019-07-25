---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f06acd154b19fbc5676645059d41fe9e6e612be3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713585"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMembers = await graphClient.Groups["{id}"].TransitiveMembers
    .Request()
    .GetAsync();

```