---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e17ef0051e83381baa2e01c9d38b566a0cbf67d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785772"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .ReapplyFilters()
    .Request()
    .PostAsync();

```