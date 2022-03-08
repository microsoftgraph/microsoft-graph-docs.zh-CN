---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc3a8d63e071cb4f13462283db1fefd03d6f1467
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338244"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Bookmark bookmark = new Bookmark();
bookmark.description = "Book a fancy vacation in Tuscany or browse museums in Florence.";

graphClient.search().bookmarks("{bookmarksId}")
    .buildRequest()
    .patch(bookmark);

```