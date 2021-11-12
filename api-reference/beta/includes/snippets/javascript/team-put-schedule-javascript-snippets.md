---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9a4a72f36c788e31136325bbfb5711d19aab7e922c4ff050fb9f99a326ac75a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103930"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schedule = {
  enabled: true,
  timeZone: 'America/Chicago'
};

await client.api('/teams/{teamId}/schedule')
    .version('beta')
    .put(schedule);

```