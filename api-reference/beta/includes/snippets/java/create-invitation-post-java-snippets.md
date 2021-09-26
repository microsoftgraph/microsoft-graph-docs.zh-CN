---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 166b459b265564e649ec719cf1f9231f2cbd8dc0
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767427"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Invitation invitation = new Invitation();
invitation.invitedUserEmailAddress = "admin@fabrikam.com";
invitation.inviteRedirectUrl = "https://myapp.contoso.com";

graphClient.invitations()
    .buildRequest()
    .post(invitation);

```