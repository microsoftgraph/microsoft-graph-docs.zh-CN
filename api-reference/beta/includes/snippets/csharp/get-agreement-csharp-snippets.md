---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bd001b4bb233fedca85bef8642a70c3eb617741d
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408499"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = await graphClient.Agreements["{id}"]
    .Request()
    .Expand("files")
    .GetAsync();

```