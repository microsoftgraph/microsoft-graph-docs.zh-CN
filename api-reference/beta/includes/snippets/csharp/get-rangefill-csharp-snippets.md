---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc5df72b076149533995b770cd5fe276bf1b582a334b6aa46039f7bd6951c56c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216014"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format.Fill
    .Request()
    .GetAsync();

```