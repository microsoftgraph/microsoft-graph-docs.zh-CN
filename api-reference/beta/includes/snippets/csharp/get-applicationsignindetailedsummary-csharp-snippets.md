---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3b3d0570f6d78a77b88c5bfdcf453dd8090d4a96
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408220"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applicationSignInDetailedSummary = await graphClient.Reports.ApplicationSignInDetailedSummary["{id}"]
    .Request()
    .GetAsync();

```