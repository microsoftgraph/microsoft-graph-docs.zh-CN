---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bae15c11393708301cc7a2efa7fa8635ad56acb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793432"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var webAccount = await graphClient.Me.Profile.WebAccounts["{webAccount-id}"]
    .Request()
    .GetAsync();

```