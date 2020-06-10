---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ae7c096f77e5d230cd4fc146f63961d5e4a24ed
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684742"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Root.Items["{item-id}"].Permissions["{perm-id}"]
    .Request()
    .DeleteAsync();

```