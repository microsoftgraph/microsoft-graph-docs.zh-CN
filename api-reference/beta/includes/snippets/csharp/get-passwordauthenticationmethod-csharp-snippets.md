---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86d1533813e0ef3ba7cf54b1015593ce7d48ed93
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806508"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var passwordAuthenticationMethod = await graphClient.Me.Authentication.PasswordMethods["{id}"]
    .Request()
    .GetAsync();

```