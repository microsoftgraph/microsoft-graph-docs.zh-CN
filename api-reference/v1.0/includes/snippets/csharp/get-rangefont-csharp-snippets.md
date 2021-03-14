---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d093c66b3cf1edd17f9d04e2a9a3409ed1bcac33
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808402"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format.Font
    .Request()
    .GetAsync();

```