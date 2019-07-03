---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 86e6cc0fd8e410e41aa3df64398930965508d4d3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463012"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSkypeForBusinessPeerToPeerActivityMinuteCounts('D7')
    .Request()
    .GetAsync();

```