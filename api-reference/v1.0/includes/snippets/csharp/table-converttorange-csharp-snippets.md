---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73c90ecd07e5f2fff958ffcf5486d8cf3a64027e45250f991ba0afdc03d75e5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333465"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .ConvertToRange()
    .Request()
    .PostAsync();

```