---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70b3de0616373d1947df9877d0c76b02a8ba4856
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209131"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _boolean = {
  messageIds: ['MC172851', 'MC167983']
};

await client.api('/admin/serviceAnnouncement/messages/unarchive')
    .version('beta')
    .post(_boolean);

```