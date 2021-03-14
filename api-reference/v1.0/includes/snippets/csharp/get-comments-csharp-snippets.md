---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c61c840a229d3b58bae162791b318ece3a8fe2c5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781892"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comments = await graphClient.Drive.Items["{driveItem-id}"].Workbook.Comments
    .Request()
    .GetAsync();

```