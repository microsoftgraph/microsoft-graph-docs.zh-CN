---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5f6aca11b059665abcc95ace2f3bf3843dad117
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971704"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthorizationPolicy authorizationPolicy = new AuthorizationPolicy();
authorizationPolicy.allowEmailVerifiedUsersToJoinOrganization = false;

graphClient.policies().authorizationPolicy()
    .buildRequest()
    .patch(authorizationPolicy);

```