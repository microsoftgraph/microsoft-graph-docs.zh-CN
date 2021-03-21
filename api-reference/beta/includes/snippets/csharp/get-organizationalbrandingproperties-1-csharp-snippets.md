---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77b7213ab4917743e3ef6135bc06470b63b368c9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955788"
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