---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c0bf7963dd0d441113f7b4e75e083d0201cfc118
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358983"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessPeerToPeerActivityMinuteCounts = await graphClient.Reports
    .GetSkypeForBusinessPeerToPeerActivityMinuteCounts("D7")
    .Request()
    .GetAsync();

```