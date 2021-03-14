---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: afba47a4b9e6d5d775985cdb561dd0790f0e55e3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809787"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var id = "id-value";

var groupId = "groupId-value";

await graphClient.Me.Onenote.Pages["{onenotePage-id}"]
    .CopyToSection(id,groupId,null,null)
    .Request()
    .PostAsync();

```