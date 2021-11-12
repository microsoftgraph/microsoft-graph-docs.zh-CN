---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19c1c417beacd339d14e0c8cc3c8653dd18a1b9437484d28407547997bcd94eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220242"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFormat = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format
    .Request()
    .GetAsync();

```