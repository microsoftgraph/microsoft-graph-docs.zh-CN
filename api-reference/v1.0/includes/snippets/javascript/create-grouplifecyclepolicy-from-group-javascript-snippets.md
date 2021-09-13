---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fd4600c7715a3c9ef953b3a7b92dde9aa0757d2d244e0a9f68e7fbec9fe8f8d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409725"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupLifecyclePolicy = {
  groupLifetimeInDays: 100,
  managedGroupTypes: 'Selected',
  alternateNotificationEmails: 'admin@contoso.com'
};

await client.api('/groupLifecyclePolicies')
    .post(groupLifecyclePolicy);

```