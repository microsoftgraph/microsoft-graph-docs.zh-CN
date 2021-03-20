---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d05b4e56b4f123ddf596eaa13484d267347d1b3e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941867"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var replies = await graphClient.Drive.Items["{driveItem-id}"].Workbook.Comments["{workbookComment-id}"].Replies
    .Request()
    .GetAsync();

```