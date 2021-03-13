---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db4f1f517251e0bb5be736e0d786a1fc70b622df
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801607"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "Sheet1!A1:D5";

var hasHeaders = true;

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables
    .Add(hasHeaders,address)
    .Request()
    .PostAsync();

```