---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2f1976ad3ef3aed914eed50cdc73f84300217bd
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338925"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Search.Bookmarks["{search.bookmark-id}"]
    .Request()
    .DeleteAsync();

```