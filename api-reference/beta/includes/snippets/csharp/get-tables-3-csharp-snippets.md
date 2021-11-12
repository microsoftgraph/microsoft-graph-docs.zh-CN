---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4243c031459ae69a64431c8a536bbe5f5fe89fd5a059ff8383e4e68f24f94d30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221276"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tables = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Tables
    .Request()
    .GetAsync();

```