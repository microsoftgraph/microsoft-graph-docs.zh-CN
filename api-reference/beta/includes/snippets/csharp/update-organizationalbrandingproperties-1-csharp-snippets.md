---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13956ffcf1212e864d56c17fe564b601a4e63cfc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943939"
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