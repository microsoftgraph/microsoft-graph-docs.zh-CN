---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 898fb6fa0ac7881593167469473fd24b03b4729659f2cbce717a1c2a0b29d766
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163748"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = 3;

var values = JsonDocument.Parse("[{}]");

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns
    .Add(index,values,null)
    .Request()
    .PostAsync();

```