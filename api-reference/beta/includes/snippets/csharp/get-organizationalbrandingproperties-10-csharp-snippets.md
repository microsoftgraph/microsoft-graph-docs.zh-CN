---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 091d758e31f7f31e3c90c1c48eba85b370c14cd1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var localizations = await graphClient.Organization["{organization-id}"].Branding.Localizations["{organizationalBrandingLocalization-id}"]
    .Request()
    .Select("SignInPageText")
    .GetAsync();

var signInPageText = localizations.SignInPageText;

```