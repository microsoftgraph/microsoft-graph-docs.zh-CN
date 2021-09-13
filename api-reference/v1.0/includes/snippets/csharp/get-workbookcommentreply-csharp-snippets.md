---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33b27d20b13c90d847642ed3136f52eca625cd6249a893150b40e8e25478f81e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105074"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookCommentReply = await graphClient.Drive.Items["{driveItem-id}"].Workbook.Comments["{workbookComment-id}"].Replies["{workbookCommentReply-id}"]
    .Request()
    .GetAsync();

```