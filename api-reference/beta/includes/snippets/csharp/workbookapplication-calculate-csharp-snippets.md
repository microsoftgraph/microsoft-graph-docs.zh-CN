---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4fd19565c8cd86cb825eb49b7e4f8c9042da8b5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779615"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calculationType = "calculationType-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Application
    .Calculate(calculationType)
    .Request()
    .PostAsync();

```