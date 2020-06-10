---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b581dd6d2df13d55af63356067072d5a5392508d
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685142"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var response = await graphClient.Me.Drive.Items["{item-id}"].Thumbnails["{thumb-id}"]["{size}"]
    .Request()
    .GetAsync();

```