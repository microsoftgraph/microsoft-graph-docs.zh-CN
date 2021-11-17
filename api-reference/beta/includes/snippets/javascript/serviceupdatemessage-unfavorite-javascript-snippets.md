---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c39192fc4da2df22c42f5737a4fc761da8555424eee90ab7dc1af9f5c2ce6a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220766"
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