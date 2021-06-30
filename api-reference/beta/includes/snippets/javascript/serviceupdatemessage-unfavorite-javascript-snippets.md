---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4241376aa6c3e49cb4da7f59d5c5681b02585d39
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _boolean = {
  messageIds: ['MC172851', 'MC167983']
};

await client.api('/admin/serviceAnnouncement/messages/unfavorite')
    .version('beta')
    .post(_boolean);

```