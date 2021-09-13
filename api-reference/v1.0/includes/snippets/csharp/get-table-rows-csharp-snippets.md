---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39acc788d65338bd846a67d5cb3ea523bcf77c7b670beb2c081cf59ca9ea1102
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158690"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rows = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows
    .Request()
    .Skip(5)
    .Top(5)
    .GetAsync();

```