---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee049cc3613c5acf7ceb72267bebeabff8cd151ee79a5383486e4b253f953703
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163359"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .HeaderRowRange()
    .Request()
    .GetAsync();

```