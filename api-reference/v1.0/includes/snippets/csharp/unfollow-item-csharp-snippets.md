---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 392f9bc62d80fadc57bfe3a4c575efb9cf00ee5564bfffd7de5f423c4086cdd8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378849"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Unfollow()
    .Request()
    .PostAsync();

```