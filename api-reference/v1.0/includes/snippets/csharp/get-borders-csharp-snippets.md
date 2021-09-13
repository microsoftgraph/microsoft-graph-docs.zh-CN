---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdd2939aae0d8cb581e155a3d0682dd7a5e200cd94bf45f8a1516ad31fdd9def
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902229"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var borders = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format.Borders
    .Request()
    .GetAsync();

```