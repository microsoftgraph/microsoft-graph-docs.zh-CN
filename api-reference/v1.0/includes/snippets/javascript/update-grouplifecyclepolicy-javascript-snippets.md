---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cbe8839c52ab2738ecbd88de52478d48850dee79191550d268131ea548d06b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333487"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupLifecyclePolicy = {
  groupLifetimeInDays: 180,
  managedGroupTypes: 'Selected',
  alternateNotificationEmails: 'admin@contoso.com'
};

await client.api('/groupLifecyclePolicies/{id}')
    .update(groupLifecyclePolicy);

```