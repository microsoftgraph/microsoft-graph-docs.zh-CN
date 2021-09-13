---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c334abf31b341450e9f8d5d4b95408b8e7ae90b523465189617744ff4df31805
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103901"
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
    .post(share);

```