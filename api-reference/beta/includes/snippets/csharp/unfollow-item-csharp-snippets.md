---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cfc7e72dc9c3dcb2b16f469f1b26908347de0f7f84c4bf7df4a8ae4e78bc2a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163158"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Unfollow()
    .Request()
    .DeleteAsync();

```