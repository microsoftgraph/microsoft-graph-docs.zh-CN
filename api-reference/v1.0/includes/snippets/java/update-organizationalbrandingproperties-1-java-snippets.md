---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cac93ecd17c691052d139d284aeeb109ac0d6089
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949336"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationalBranding organizationalBranding = new OrganizationalBranding();
organizationalBranding.signInPageText = "Default";
organizationalBranding.usernameHintText = "DefaultHint";

graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding()
    .buildRequest()
    .patch(organizationalBranding);

```