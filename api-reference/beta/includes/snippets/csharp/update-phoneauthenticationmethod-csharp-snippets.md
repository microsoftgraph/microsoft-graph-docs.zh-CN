---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c40b375bac3cebb27da6be832a8da877550e810
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803309"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var phoneAuthenticationMethod = new PhoneAuthenticationMethod
{
    PhoneNumber = "+1 2065555554",
    PhoneType = AuthenticationPhoneType.Mobile
};

await graphClient.Me.Authentication.PhoneMethods["{phoneAuthenticationMethod-id}"]
    .Request()
    .PutAsync(phoneAuthenticationMethod);

```