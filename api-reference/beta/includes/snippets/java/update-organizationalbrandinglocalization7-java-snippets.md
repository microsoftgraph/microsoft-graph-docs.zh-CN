---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4b5b82d1f20534be61f4a90c6c8319b6cb0e464
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996569"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationalBrandingLocalization organizationalBrandingLocalization = new OrganizationalBrandingLocalization();
organizationalBrandingLocalization.signInPageText = "Welcome to Contoso France.";
organizationalBrandingLocalization.usernameHintText = " ";

graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding().localizations("fr-FR")
    .buildRequest()
    .patch(organizationalBrandingLocalization);

```