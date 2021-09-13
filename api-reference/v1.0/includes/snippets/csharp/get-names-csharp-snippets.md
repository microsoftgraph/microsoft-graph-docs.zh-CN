---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12d1a4f4895e004423344b4a32733de2d30f31143c377d8fd1c7527ad4e0f4f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162056"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var names = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names
    .Request()
    .GetAsync();

```