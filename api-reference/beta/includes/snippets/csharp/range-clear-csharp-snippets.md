---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a5e60d90dc1ed7bde83d7475916a55c60afcb7f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800993"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applyTo = "applyTo-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .Clear(applyTo)
    .Request()
    .PostAsync();

```