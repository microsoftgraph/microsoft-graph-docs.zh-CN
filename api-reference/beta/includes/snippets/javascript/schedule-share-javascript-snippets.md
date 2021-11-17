---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf2c442c8dad3f41df916ba073a3349989a045a7b8035b6cf4013c5dd014e349
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158484"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const share = {
  notifyTeam: true,
  startDateTime: '2018-10-08T00:00:00.000Z',
  endDateTime: '2018-10-15T00:00:00.000Z'
};

await client.api('/teams/{teamId}/schedule/share')
    .version('beta')
    .post(share);

```