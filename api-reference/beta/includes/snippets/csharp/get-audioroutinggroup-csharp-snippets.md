---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3e1c221144b6e276f8692c7691e8c0f600dc6976
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933802"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var audioRoutingGroup = await graphClient.App.Calls["{id}"].AudioRoutingGroups["{id}"]
    .Request()
    .GetAsync();

```