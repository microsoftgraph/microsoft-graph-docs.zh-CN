---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1afa4e6ded51a3fd331805b45f53a366a86d4cf9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808230"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableSort = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Sort
    .Request()
    .GetAsync();

```