---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e8b965cef208cf46c4dd126ed60ca66291f0159
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806456"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Authentication.PhoneMethods["3179e48a-750b-4051-897c-87b9720928f7"]
    .DisableSmsSignIn()
    .Request()
    .PostAsync();

```