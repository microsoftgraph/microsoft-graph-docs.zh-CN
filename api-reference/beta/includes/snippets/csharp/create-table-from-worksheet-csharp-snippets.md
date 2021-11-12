---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ea70324bbd58ea9c1095b5b8d007195e82d0ccba83ea46e8fc6b490c4936e94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163881"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "";

var hasHeaders = false;

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Tables
    .Add(hasHeaders,address)
    .Request()
    .PostAsync();

```