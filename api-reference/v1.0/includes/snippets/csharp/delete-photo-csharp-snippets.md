---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 62c6d0e7a1356efe68e04fa2867737c6da1cce53
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732785"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{id|userPrincipalName}"].Photo
    .Request()
    .DeleteAsync();

```