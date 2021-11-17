---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7634e80878946fc420b4241562eaa45629fc92e6c68b69c87b8fcfe4383b5948
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903298"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _boolean = {
  messageIds: ['MC172851', 'MC167983']
};

await client.api('/admin/serviceAnnouncement/messages/archive')
    .version('beta')
    .post(_boolean);

```