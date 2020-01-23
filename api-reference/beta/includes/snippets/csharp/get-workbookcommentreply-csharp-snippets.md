---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ee719e406a47a4ee4d527122220386bdf802b4b
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41497133"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookCommentReply = await graphClient.Drive.Items["{id}"].Workbook.Comments["{id}"].Replies["{id}"]
    .Request()
    .GetAsync();

```