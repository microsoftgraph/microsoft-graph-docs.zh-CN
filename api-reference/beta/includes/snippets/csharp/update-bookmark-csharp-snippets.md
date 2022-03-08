---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd027a9b00ffb4d5c5d729c5b018ef7ca21629c4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338247"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookmark = new Microsoft.Graph.Search.Bookmark
{
    Description = "Book a fancy vacation in Tuscany or browse museums in Florence."
};

await graphClient.Search.Bookmarks["{search.bookmark-id}"]
    .Request()
    .UpdateAsync(bookmark);

```