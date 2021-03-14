---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c42f47815571a78985dcf08df49495ea94d8d5bd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782686"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var id = "id-value";

var groupId = "groupId-value";

var renameAs = "renameAs-value";

await graphClient.Me.Onenote.Sections["{onenoteSection-id}"]
    .CopyToSectionGroup(id,groupId,renameAs,null,null)
    .Request()
    .PostAsync();

```