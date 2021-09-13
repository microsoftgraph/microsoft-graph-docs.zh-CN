---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa9b3378a9cf04a5f04ee31ecc166fe228190fca27ac00db747d73317f41560a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105315"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns
    .Request()
    .Skip(5)
    .Top(5)
    .GetAsync();

```