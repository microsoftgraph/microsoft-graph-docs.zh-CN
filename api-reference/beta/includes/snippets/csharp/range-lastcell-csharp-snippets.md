---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c400f4efc3877350e1986c71d678c2b2a7fd84d60602c51402f3f81b9abd6ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273940"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .LastCell()
    .Request()
    .GetAsync();

```