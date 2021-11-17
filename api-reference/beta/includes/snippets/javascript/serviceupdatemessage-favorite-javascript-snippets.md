---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c26a1cb2801182222d81fe54e634048504ac97ec7ef11eaca8a84977b2e4fbea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903293"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _boolean = {
  messageIds: ['MC172851', 'MC167983']
};

await client.api('/admin/serviceAnnouncement/messages/favorite')
    .version('beta')
    .post(_boolean);

```