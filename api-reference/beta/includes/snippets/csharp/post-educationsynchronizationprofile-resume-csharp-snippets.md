---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1193daaf5dc8fbabb1000952d3b2ba15a0ffed6c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616491"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{id}"]
    .Resume()
    .Request()
    .PostAsync();

```