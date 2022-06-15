---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06618a5bd7149cc13d26d0c9b384625d83636c5774aa751abf2d90119a8d76e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220819"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "Updating the latest guidelines";

await graphClient.Drives["{drive-id}"].Items["{driveItem-id}"]
    .Checkin(null,comment)
    .Request()
    .PostAsync();

```