---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a991c4eca84a8e1f16412e6f79724e7500882ee2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968542"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupLifecyclePolicy groupLifecyclePolicy = new GroupLifecyclePolicy();
groupLifecyclePolicy.groupLifetimeInDays = 180;
groupLifecyclePolicy.managedGroupTypes = "Selected";
groupLifecyclePolicy.alternateNotificationEmails = "admin@contoso.com";

graphClient.groupLifecyclePolicies("{id}")
    .buildRequest()
    .patch(groupLifecyclePolicy);

```