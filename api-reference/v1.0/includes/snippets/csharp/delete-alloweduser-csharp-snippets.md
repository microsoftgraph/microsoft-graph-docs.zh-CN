---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee0970af2a0cbc3f2b4fdad66b0f7ddedeff9873
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771755"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Shares["{printerShare-id}"].AllowedUsers["{user-id}"].Reference
    .Request()
    .DeleteAsync();

```