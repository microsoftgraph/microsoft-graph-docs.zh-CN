---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b17ddedce50eb34949af28136a8eba27e54807120a92fb21d2f73f4562727ea4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409503"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupId = "groupId-value";

var renameAs = "renameAs-value";

await graphClient.Me.Onenote.Notebooks["{notebook-id}"]
    .CopyNotebook(groupId,renameAs,null,null,null)
    .Request()
    .PostAsync();

```