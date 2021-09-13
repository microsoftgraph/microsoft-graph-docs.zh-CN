---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d66bac9c2992039b36d052d19bad689b50ad095318a41477f4e6ec1fc337a27
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902221"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var id = "id-value";

var groupId = "groupId-value";

var renameAs = "renameAs-value";

await graphClient.Me.Onenote.Sections["{onenoteSection-id}"]
    .CopyToNotebook(id,groupId,renameAs,null,null)
    .Request()
    .PostAsync();

```