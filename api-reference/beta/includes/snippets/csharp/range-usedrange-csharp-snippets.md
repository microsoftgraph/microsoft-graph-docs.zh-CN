---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9338923848cb46d8b663d6e4bfd7745defceeda6c8cd18359fb68d33fa4d7dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220494"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .UsedRange()
    .Request()
    .GetAsync();

```