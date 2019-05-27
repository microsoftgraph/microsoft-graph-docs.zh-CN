---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 62c6d0e7a1356efe68e04fa2867737c6da1cce53
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437767"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{id|userPrincipalName}"].Photo
    .Request()
    .DeleteAsync();

```