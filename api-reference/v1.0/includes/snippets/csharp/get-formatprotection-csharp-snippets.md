---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9883059db208af906e47ab0ee59073ac5691344278e09d69aa2efbb6802caef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218404"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookFormatProtection = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format.Protection
    .Request()
    .GetAsync();

```