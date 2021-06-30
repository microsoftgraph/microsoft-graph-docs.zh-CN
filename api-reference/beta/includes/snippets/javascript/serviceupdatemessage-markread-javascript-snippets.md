---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0855331d2eddca17b48ede6e8d7b7fc91ca2c23f
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209358"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _boolean = {
  messageIds: ['MC172851', 'MC167983']
};

await client.api('/admin/serviceAnnouncement/messages/markRead')
    .version('beta')
    .post(_boolean);

```