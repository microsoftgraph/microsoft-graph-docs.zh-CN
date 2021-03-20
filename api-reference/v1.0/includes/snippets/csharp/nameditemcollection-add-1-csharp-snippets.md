---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90351fc6a4e74adaf6b443ec9d81e38cf4e8bec0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949771"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var name = "test5";

var reference = "=Sheet1!$F$15:$N$27";

var comment = "Comment for the named item";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names
    .Add(name,reference,comment)
    .Request()
    .PostAsync();

```