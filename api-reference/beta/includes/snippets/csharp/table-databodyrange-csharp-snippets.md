---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9bd5c61be47cfe790ab6270e3e84443ddaf64e508b1597439fd7f15cf785928
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161656"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .DataBodyRange()
    .Request()
    .GetAsync();

```