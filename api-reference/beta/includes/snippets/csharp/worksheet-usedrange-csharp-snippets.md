---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a190c340825b1d4364dd1471ba8aa45f36b164b8da39d301bbb7318c4371e44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274112"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"]
    .UsedRange(true)
    .Request()
    .GetAsync();

```