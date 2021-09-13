---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 988d5c3e2f56b56d1a296a31888940b77a64e4192e5182b7739142c69397d6ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332956"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .LastRow()
    .Request()
    .GetAsync();

```