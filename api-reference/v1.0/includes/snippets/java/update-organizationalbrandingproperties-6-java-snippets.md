---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 296d861790b6b700bc0dfc16ab50ca2e5373a0b5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959724"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationalBrandingLocalization organizationalBrandingLocalization = new OrganizationalBrandingLocalization();
organizationalBrandingLocalization.backgroundColor = "#00000F";
organizationalBrandingLocalization.signInPageText = "fr";

graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding().localizations("fr")
    .buildRequest()
    .patch(organizationalBrandingLocalization);

```