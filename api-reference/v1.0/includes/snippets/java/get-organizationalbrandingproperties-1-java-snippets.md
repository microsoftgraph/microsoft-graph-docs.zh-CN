---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12a2f12303d16828e3fe72b2aa0a362f1eb81ea29131753dc339530dfb11e41c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220557"
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