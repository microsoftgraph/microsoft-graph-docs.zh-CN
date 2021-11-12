---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b23de5f63c1911f7a7ac53baade0b4e6032ca4b44269a363e2d265e0058424f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106585"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var names = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Names
    .Request()
    .GetAsync();

```