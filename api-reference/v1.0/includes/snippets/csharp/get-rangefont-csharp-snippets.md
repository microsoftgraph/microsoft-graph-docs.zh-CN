---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e2705e50353174b4d632b95ef61e9141b10876b14c72045747c000831d5f398
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409332"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format.Font
    .Request()
    .GetAsync();

```