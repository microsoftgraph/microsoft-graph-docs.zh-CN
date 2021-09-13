---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7412a4dbdda7ef7f413cba041260706231e2fca75b183be153ade1c76b789005
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333486"
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