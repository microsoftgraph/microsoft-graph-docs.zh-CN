---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b7bd177cda7a951ddf8501d9943851fa1b93b66
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225511"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attributeSets = await graphClient.Directory.AttributeSets
    .Request()
    .OrderBy("id")
    .GetAsync();

```