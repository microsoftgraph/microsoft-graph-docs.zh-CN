---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffdfc65e2b6f826d139dd3fcdf96dbff494c58bc75de4bdae488eb8c1d92134e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163750"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var values = JsonDocument.Parse("[[1,2,3],[4,5,6]]");

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows
    .Add(null,values)
    .Request()
    .PostAsync();

```