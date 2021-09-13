---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed88c9681a1f26010f94a4c9da8954c1cccae7d09cdaac971c38ed5c0b9742e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409085"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

using var stream = new System.IO.MemoryStream(Encoding.UTF8.GetBytes(@"The contents of the file goes here."));

await graphClient.Me.Drive.Items["{driveItem-id}"].Content
    .Request()
    .PutAsync<DriveItem>(stream);

```