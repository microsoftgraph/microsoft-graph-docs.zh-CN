---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b2167e3c013a350b7f7cefc3d7e3588c112b0f6386faa497986c0615edf32d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278527"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Invitation invitation = new Invitation();
invitation.invitedUserEmailAddress = "yyy@test.com";
invitation.inviteRedirectUrl = "https://myapp.contoso.com";

graphClient.invitations()
    .buildRequest()
    .post(invitation);

```