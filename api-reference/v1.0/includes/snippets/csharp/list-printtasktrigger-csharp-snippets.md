---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 771cd028620926ef262b698a1cca3df2e0ac0602
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771909"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskTriggers = await graphClient.Print.Printers["{printer-id}"].TaskTriggers
    .Request()
    .GetAsync();

```