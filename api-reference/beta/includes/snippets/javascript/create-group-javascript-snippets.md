---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 971d6588cd317d572be3b7177773761f7e664ce39562987e12ac9feeac03551f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277443"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: 'Self help community for golf',
  displayName: 'Golf Assist',
  groupTypes: [
    'Unified'
  ],
  mailEnabled: true,
  mailNickname: 'golfassist',
  securityEnabled: false
};

await client.api('/groups')
    .version('beta')
    .post(group);

```