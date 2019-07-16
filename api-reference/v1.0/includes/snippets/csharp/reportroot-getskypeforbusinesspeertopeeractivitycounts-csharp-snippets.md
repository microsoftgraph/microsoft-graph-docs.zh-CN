---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 17e09571630818fd7cb215c38d6c7513864b56e7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738196"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSkypeForBusinessPeerToPeerActivityCounts('D7')
    .Request()
    .GetAsync();

```