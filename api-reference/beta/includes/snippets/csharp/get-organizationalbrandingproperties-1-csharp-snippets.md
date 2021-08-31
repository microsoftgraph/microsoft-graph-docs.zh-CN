---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64c049d77d34f0fdc792455b0e8706919c518117b1ecd5730db80b6d2d85a4c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221358"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBranding = new OrganizationalBranding
{
    BackgroundColor = "#FFFF33",
    SignInPageText = "Welcome",
    UsernameHintText = "hint"
};

await graphClient.Organization["{organization-id}"].Branding
    .Request()
    .PutAsync(organizationalBranding);

```