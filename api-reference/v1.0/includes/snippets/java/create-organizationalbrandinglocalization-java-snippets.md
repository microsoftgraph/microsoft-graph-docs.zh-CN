---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7aa9a82b678a49b4bb2dc6fd6b13b91e63d64923
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996961"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationalBrandingLocalization organizationalBrandingLocalization = new OrganizationalBrandingLocalization();
organizationalBrandingLocalization.backgroundColor = "#00000F";
organizationalBrandingLocalization.id = "fr-FR";
organizationalBrandingLocalization.signInPageText = " ";

graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding().localizations()
    .buildRequest()
    .post(organizationalBrandingLocalization);

```