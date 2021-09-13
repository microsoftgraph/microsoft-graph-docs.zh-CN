---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 465c880fbfb15de6c0db16ec74985fddc9bb06a5ae0f938cdc19692b86e09241
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158687"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .ReapplyFilters()
    .Request()
    .PostAsync();

```