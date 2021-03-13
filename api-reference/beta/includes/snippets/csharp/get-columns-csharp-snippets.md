---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74d2dd12168a5e5dde6251a31ec2863e7a15b348
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786470"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns
    .Request()
    .Skip(5)
    .Top(5)
    .GetAsync();

```