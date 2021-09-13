---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ac5416478f0b6ca9d00f5410eae38a2a8efa4b20d096ff2cd857897ea431eb1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409770"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"]
    .Request()
    .DeleteAsync();

```