---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ecd58d5f3369470f4ef65f28d73a23172b9edcd84c8c4f3911b284c14ed3edf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162389"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .EntireColumn()
    .Request()
    .GetAsync();

```