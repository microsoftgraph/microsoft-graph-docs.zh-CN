---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d25ea76177390e844d0fb2e28cbda6faf61a5c53ae56deecc8ad7ad57a3655f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903999"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var name = "name-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets
    .Add(name)
    .Request()
    .PostAsync();

```