---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04d8bf66aef0d4c88a6b0924c4fdb11bf7d5f5ba
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210793"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _boolean = {
  messageIds: ['MC172851', 'MC167983']
};

await client.api('/admin/serviceAnnouncement/messages/markUnread')
    .version('beta')
    .post(_boolean);

```