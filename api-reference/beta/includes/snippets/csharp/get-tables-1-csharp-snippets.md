---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d47c1f0fc187617424d68c05305bcd99b00b22a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952831"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tables = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables
    .Request()
    .GetAsync();

```