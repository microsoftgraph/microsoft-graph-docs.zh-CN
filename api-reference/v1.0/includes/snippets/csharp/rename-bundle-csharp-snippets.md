---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f17580290f970818f81b8d044543aa48c9e09e1
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758053"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "Shared legal agreements"
};

await graphClient.Drive.Items["{driveItem-id}"]
    .Request()
    .UpdateAsync(driveItem);

```