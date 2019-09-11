---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2432c7f0fba4d7b1741161e3402fac86b1d00b11
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838707"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookCommentReply = await graphClient.Drive.Root.Workbook.Comments["{id}"].Replies["{id}"]
    .Request()
    .GetAsync();

```