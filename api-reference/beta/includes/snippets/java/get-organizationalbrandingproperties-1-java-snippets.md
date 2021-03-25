---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af877c0b34d8adf8ceeeddc9fc29c3ccd0b2e173
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211183"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationalBranding organizationalBranding = new OrganizationalBranding();
organizationalBranding.backgroundColor = "#FFFF33";
organizationalBranding.signInPageText = "Welcome";
organizationalBranding.usernameHintText = "hint";

graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding()
    .buildRequest()
    .put(organizationalBranding);

```