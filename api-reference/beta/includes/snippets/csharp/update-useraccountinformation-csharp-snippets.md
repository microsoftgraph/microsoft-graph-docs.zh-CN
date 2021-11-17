---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37055ffe2b948ac3aa1a2a09a027b01f17899e295ac695388ea1eb0d00d9f25d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903272"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAccountInformation = new UserAccountInformation
{
    CountryCode = "NO"
};

await graphClient.Me.Profile.Account["{userAccountInformation-id}"]
    .Request()
    .UpdateAsync(userAccountInformation);

```