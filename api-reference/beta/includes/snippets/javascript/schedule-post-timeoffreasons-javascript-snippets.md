---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42869011002e867f5e91959eb097d82160e9198c2e3161d32abf1fd5368a598a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274130"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeOffReason = {
  displayName: 'Vacation',
  iconType: 'plane',
  isActive: true
};

await client.api('/teams/{teamId}/schedule/timeOffReasons')
    .version('beta')
    .post(timeOffReason);

```