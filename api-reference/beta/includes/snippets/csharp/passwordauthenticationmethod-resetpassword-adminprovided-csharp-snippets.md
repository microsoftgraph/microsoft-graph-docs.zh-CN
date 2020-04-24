---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee4ca959dab480b7a23f0286fd6e161a14d2bc9f
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805973"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var newPassword = "newPassword-value";

await graphClient.Users["{id}"].Authentication.PasswordMethods["{id}"]
    .ResetPassword(newPassword,null)
    .Request()
    .PostAsync();

```