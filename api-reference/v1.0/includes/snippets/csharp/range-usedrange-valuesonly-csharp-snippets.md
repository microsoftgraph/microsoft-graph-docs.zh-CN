---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d42590703509a0666e78ad67340f4311d200f4d992657e5c6a8070e920a0bba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .UsedRange(true)
    .Request()
    .GetAsync();

```