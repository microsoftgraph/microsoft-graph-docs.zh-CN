---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dba395b2a0b6fdb9223a6b85a1eb6498ee40eef3
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870379"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Protection
    .Unprotect()
    .Request()
    .PostAsync();

```