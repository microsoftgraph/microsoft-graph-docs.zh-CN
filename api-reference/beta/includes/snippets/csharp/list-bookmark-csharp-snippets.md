---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53493a98edf8e9be885a451c8f456f304f5148bf
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338861"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookmarks = await graphClient.Search.Bookmarks
    .Request()
    .GetAsync();

```