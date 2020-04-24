---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 936a327a68b505e2c8e799ae3847230e20ece102
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805840"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var phoneAuthenticationMethod = new PhoneAuthenticationMethod
{
    PhoneNumber = "+1 2065555554",
    PhoneType = AuthenticationPhoneType.Mobile
};

await graphClient.Me.Authentication.PhoneMethods["3179e48a-750b-4051-897c-87b9720928f7"]
    .Request()
    .PutAsync(phoneAuthenticationMethod);

```