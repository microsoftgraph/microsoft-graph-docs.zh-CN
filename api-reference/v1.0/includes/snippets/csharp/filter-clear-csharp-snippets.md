---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c1560cd01b1b859a1befac3e179e922e5db1b1ab5f667dc580169ef3866f56b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221173"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns["{workbookTableColumn-id}"].Filter
    .Clear()
    .Request()
    .PostAsync();

```