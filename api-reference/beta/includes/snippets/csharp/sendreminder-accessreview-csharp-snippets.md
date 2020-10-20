---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d818ace631e591ea0ae53d75a939a1627dfc7394
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605908"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["2975E9B5-44CE-4E71-93D3-30F03B5AA992"]
    .SendReminder()
    .Request()
    .PostAsync();

```