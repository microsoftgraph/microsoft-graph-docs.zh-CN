---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3dc538065230afa645ad5aa7cc88652c9c653d8ed25c3850aeb7b82c3984999a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220549"
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