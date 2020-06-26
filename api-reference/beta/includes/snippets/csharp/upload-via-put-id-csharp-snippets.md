---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fecfcecb31e62ea2924a065e67bd3c2b84b6c7d2
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44900286"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

using var stream = new System.IO.MemoryStream(Encoding.UTF8.GetBytes("The contents of the file goes here."));

await graphClient.Me.Drive.Items["{item-id}"].Content
    .Request()
    .PutAsync<DriveItem>(stream);

```