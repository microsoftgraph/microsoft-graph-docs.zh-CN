---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d818ace631e591ea0ae53d75a939a1627dfc7394
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710858"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["2975E9B5-44CE-4E71-93D3-30F03B5AA992"]
    .SendReminder()
    .Request()
    .PostAsync();

```