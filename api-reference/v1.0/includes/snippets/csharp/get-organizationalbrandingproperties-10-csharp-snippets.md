---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a908294306f97454c162d583870ab3a7fa6ad6e3baa96b670d8d97ae9cbd2e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277129"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var localizations = await graphClient.Organization["{organization-id}"].Branding.Localizations["{organizationalBrandingLocalization-id}"]
    .Request()
    .Select("SignInPageText")
    .GetAsync();

var signInPageText = localizations.SignInPageText;

```