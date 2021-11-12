---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 488bcf022ba032c5d8db0e67ce38d8eb6cec313f376dea4e00e23f5d06cba8e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164247"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns["{workbookTableColumn-id}"]
    .HeaderRowRange()
    .Request()
    .GetAsync();

```