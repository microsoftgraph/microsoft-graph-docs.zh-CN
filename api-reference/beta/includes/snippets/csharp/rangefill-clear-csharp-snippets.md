---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b769552d0b9b860d4a6aa802b799411d15318708
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614700"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format.Fill
    .Clear()
    .Request()
    .PostAsync();

```