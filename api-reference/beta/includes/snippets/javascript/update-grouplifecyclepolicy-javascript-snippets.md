---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edb28cf45cd96866fad549b685f73a05d554a40eac82270d1800d6963ba65cc1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273881"
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
    .version('beta')
    .update(groupLifecyclePolicy);

```