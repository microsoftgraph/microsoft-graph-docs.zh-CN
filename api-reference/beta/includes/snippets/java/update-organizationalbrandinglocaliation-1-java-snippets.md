---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6dd5be0af790d3949c83bdac7c0fa583e4d0d5a
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995574"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationalBranding organizationalBranding = new OrganizationalBranding();
organizationalBranding.signInPageText = "Default";
organizationalBranding.usernameHintText = "DefaultHint";

graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding()
    .buildRequest()
    .patch(organizationalBranding);

```