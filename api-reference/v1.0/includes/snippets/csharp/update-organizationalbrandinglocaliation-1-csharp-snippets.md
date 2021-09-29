---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13956ffcf1212e864d56c17fe564b601a4e63cfc
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995324"
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