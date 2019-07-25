---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ef6caa3f9a541be3e7e525818b5079343c77bf26
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714731"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversation = await graphClient.Groups["{id}"].Conversations["{id}"]
    .Request()
    .GetAsync();

```