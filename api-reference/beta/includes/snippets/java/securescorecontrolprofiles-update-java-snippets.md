---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb4fae09692ed99a0a74fe68e7190bf35d26fd179bed068466dabc99695c5f17
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163923"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecureScoreControlProfile secureScoreControlProfile = new SecureScoreControlProfile();
secureScoreControlProfile.controlStateUpdates = "controlStateUpdates-value";

graphClient.security().secureScoreControlProfiles("AdminMFA")
    .buildRequest()
    .patch(secureScoreControlProfile);

```