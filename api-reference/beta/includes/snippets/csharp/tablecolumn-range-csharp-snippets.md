---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7341e7b493ff5d60ff127aa7ba53ec8a8feb8acfb0f6ccabc083f008ba80d076
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163067"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns["{workbookTableColumn-id}"]
    .Range()
    .Request()
    .GetAsync();

```