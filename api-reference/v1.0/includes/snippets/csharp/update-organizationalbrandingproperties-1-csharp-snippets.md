---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 555cc69ca7f2c1cee085e3165b9636da7bb17a7548c9621508c6c98ca12a79e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101316"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBranding = new OrganizationalBranding
{
    SignInPageText = "Default",
    UsernameHintText = "DefaultHint"
};

await graphClient.Organization["{organization-id}"].Branding
    .Request()
    .UpdateAsync(organizationalBranding);

```