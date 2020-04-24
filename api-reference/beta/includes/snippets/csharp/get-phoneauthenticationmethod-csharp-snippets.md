---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06f7b3b9e09faeab39dc3d1ccd8f3b57fa4fc8c5
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806423"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var phoneAuthenticationMethod = await graphClient.Me.Authentication.PhoneMethods["3179e48a-750b-4051-897c-87b9720928f7"]
    .Request()
    .GetAsync();

```