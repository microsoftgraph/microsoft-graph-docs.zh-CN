---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd2c14a91c542acd5b47b673fe8cf6256b07992b335461e185971847a5211476
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332237"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .ClearFilters()
    .Request()
    .PostAsync();

```